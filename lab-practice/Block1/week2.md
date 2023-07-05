Week 2
================
Jeanette Choong
2/6/2020

``` r
library(tidyverse)
library(here)
```

``` r
sales <- read_csv(here::here("data/hdb_resale_2015_onwards.csv"))
```

``` r
sales %>%  glimpse()
```

    ## Observations: 79,100
    ## Variables: 11
    ## $ month               <chr> "2015-01", "2015-01", "2015-01", "2015-01", …
    ## $ town                <chr> "ANG MO KIO", "ANG MO KIO", "ANG MO KIO", "A…
    ## $ flat_type           <chr> "3 ROOM", "3 ROOM", "3 ROOM", "3 ROOM", "3 R…
    ## $ block               <chr> "174", "541", "163", "446", "557", "603", "7…
    ## $ street_name         <chr> "ANG MO KIO AVE 4", "ANG MO KIO AVE 10", "AN…
    ## $ storey_range        <chr> "07 TO 09", "01 TO 03", "01 TO 03", "01 TO 0…
    ## $ floor_area_sqm      <dbl> 60, 68, 69, 68, 68, 67, 68, 68, 67, 68, 67, …
    ## $ flat_model          <chr> "Improved", "New Generation", "New Generatio…
    ## $ lease_commence_date <dbl> 1986, 1981, 1980, 1979, 1980, 1980, 1980, 19…
    ## $ remaining_lease     <dbl> 70, 65, 64, 63, 64, 64, 64, 65, 62, 69, 60, …
    ## $ resale_price        <dbl> 255000, 275000, 285000, 290000, 290000, 2900…

``` r
library(lubridate)
```

    ## 
    ## Attaching package: 'lubridate'

    ## The following object is masked from 'package:here':
    ## 
    ##     here

    ## The following object is masked from 'package:base':
    ## 
    ##     date

``` r
library(forcats)

sales %>% 
  mutate(month = ymd(month, truncated = 1), 
         flat_type = as_factor(flat_type), 
         storey_range = as_factor(storey_range),
         flat_model = as_factor(flat_model))
```

    ## # A tibble: 79,100 x 11
    ##    month      town  flat_type block street_name storey_range floor_area_sqm
    ##    <date>     <chr> <fct>     <chr> <chr>       <fct>                 <dbl>
    ##  1 2015-01-01 ANG … 3 ROOM    174   ANG MO KIO… 07 TO 09                 60
    ##  2 2015-01-01 ANG … 3 ROOM    541   ANG MO KIO… 01 TO 03                 68
    ##  3 2015-01-01 ANG … 3 ROOM    163   ANG MO KIO… 01 TO 03                 69
    ##  4 2015-01-01 ANG … 3 ROOM    446   ANG MO KIO… 01 TO 03                 68
    ##  5 2015-01-01 ANG … 3 ROOM    557   ANG MO KIO… 07 TO 09                 68
    ##  6 2015-01-01 ANG … 3 ROOM    603   ANG MO KIO… 07 TO 09                 67
    ##  7 2015-01-01 ANG … 3 ROOM    709   ANG MO KIO… 01 TO 03                 68
    ##  8 2015-01-01 ANG … 3 ROOM    333   ANG MO KIO… 01 TO 03                 68
    ##  9 2015-01-01 ANG … 3 ROOM    109   ANG MO KIO… 01 TO 03                 67
    ## 10 2015-01-01 ANG … 3 ROOM    564   ANG MO KIO… 13 TO 15                 68
    ## # … with 79,090 more rows, and 4 more variables: flat_model <fct>,
    ## #   lease_commence_date <dbl>, remaining_lease <dbl>, resale_price <dbl>

# What is the earlier lease commencement date and where are these flats located?

1966, Jurong East

``` r
sales %>% 
  arrange(lease_commence_date) %>% 
  select(town, lease_commence_date)
```

    ## # A tibble: 79,100 x 2
    ##    town        lease_commence_date
    ##    <chr>                     <dbl>
    ##  1 JURONG EAST                1966
    ##  2 JURONG EAST                1966
    ##  3 JURONG EAST                1966
    ##  4 JURONG EAST                1966
    ##  5 JURONG EAST                1966
    ##  6 JURONG EAST                1966
    ##  7 JURONG EAST                1966
    ##  8 JURONG EAST                1966
    ##  9 JURONG EAST                1966
    ## 10 GEYLANG                    1967
    ## # … with 79,090 more rows

# What are the largest HDB flats in Singapore? How much did they sell for?

3 room terrace flats in Kallang/Whampoa, sold for between S$830,000 -
S$1,185,000.

``` r
sales %>% 
  arrange(-floor_area_sqm)
```

    ## # A tibble: 79,100 x 11
    ##    month town  flat_type block street_name storey_range floor_area_sqm
    ##    <chr> <chr> <chr>     <chr> <chr>       <chr>                 <dbl>
    ##  1 2015… KALL… 3 ROOM    53    JLN MA'MOR  01 TO 03                280
    ##  2 2016… KALL… 3 ROOM    57    JLN MA'MOR  01 TO 03                259
    ##  3 2017… KALL… 3 ROOM    65    JLN MA'MOR  01 TO 03                249
    ##  4 2015… KALL… 3 ROOM    60    JLN BAHAGIA 01 TO 03                241
    ##  5 2018… KALL… 3 ROOM    41    JLN BAHAGIA 01 TO 03                237
    ##  6 2017… KALL… 3 ROOM    38    JLN BAHAGIA 01 TO 03                215
    ##  7 2017… CHOA… EXECUTIVE 641   CHOA CHU K… 16 TO 18                215
    ##  8 2018… CHOA… EXECUTIVE 639   CHOA CHU K… 10 TO 12                215
    ##  9 2016… BISH… EXECUTIVE 446   BRIGHT HIL… 07 TO 09                199
    ## 10 2015… WOOD… EXECUTIVE 330   WOODLANDS … 07 TO 09                192
    ## # … with 79,090 more rows, and 4 more variables: flat_model <chr>,
    ## #   lease_commence_date <dbl>, remaining_lease <dbl>, resale_price <dbl>

# What is the most expensive flat in Punggol?

5-room Premium Apartment Loft at Blk 305B Punggol Rd, between 16-18
storey.

``` r
sales %>% 
  filter(town == "PUNGGOL") %>% 
  arrange(-resale_price)
```

    ## # A tibble: 4,386 x 11
    ##    month town  flat_type block street_name storey_range floor_area_sqm
    ##    <chr> <chr> <chr>     <chr> <chr>       <chr>                 <dbl>
    ##  1 2018… PUNG… 5 ROOM    305B  PUNGGOL RD  16 TO 18                147
    ##  2 2017… PUNG… 5 ROOM    267A  PUNGGOL FI… 16 TO 18                149
    ##  3 2016… PUNG… 5 ROOM    270A  PUNGGOL FI… 16 TO 18                149
    ##  4 2018… PUNG… 5 ROOM    306D  PUNGGOL DR  16 TO 18                147
    ##  5 2016… PUNG… 5 ROOM    305A  PUNGGOL RD  16 TO 18                147
    ##  6 2016… PUNG… 5 ROOM    305D  PUNGGOL DR  16 TO 18                147
    ##  7 2015… PUNG… 5 ROOM    306A  PUNGGOL PL  16 TO 18                147
    ##  8 2018… PUNG… 5 ROOM    272A  PUNGGOL WA… 16 TO 18                116
    ##  9 2018… PUNG… 5 ROOM    271C  PUNGGOL WA… 07 TO 09                116
    ## 10 2016… PUNG… 5 ROOM    270B  PUNGGOL FI… 16 TO 18                149
    ## # … with 4,376 more rows, and 4 more variables: flat_model <chr>,
    ## #   lease_commence_date <dbl>, remaining_lease <dbl>, resale_price <dbl>

# Which town has, on average, the largest flats (by floor area)?

Ang Mo Kio

``` r
sales %>% 
  arrange(-floor_area_sqm) %>% 
  group_by(town) %>% 
  summarise(average_resale_price = mean(resale_price))
```

    ## # A tibble: 26 x 2
    ##    town          average_resale_price
    ##    <chr>                        <dbl>
    ##  1 ANG MO KIO                 416431.
    ##  2 BEDOK                      412098.
    ##  3 BISHAN                     630955.
    ##  4 BUKIT BATOK                384390.
    ##  5 BUKIT MERAH                555017.
    ##  6 BUKIT PANJANG              420138.
    ##  7 BUKIT TIMAH                711795.
    ##  8 CENTRAL AREA               653313.
    ##  9 CHOA CHU KANG              390059.
    ## 10 CLEMENTI                   459451.
    ## # … with 16 more rows

# Which town has, on average, the cheapest flats per square meter?

Choa Chu Kang

``` r
sales %>% 
mutate(cost_sqm = (resale_price/floor_area_sqm)) %>% 
  group_by(town) %>% 
  summarise(cost_sqm_town = mean(cost_sqm)) %>% 
  arrange(cost_sqm_town)
```

    ## # A tibble: 26 x 2
    ##    town          cost_sqm_town
    ##    <chr>                 <dbl>
    ##  1 CHOA CHU KANG         3529.
    ##  2 WOODLANDS             3625.
    ##  3 SEMBAWANG             3729.
    ##  4 YISHUN                3907.
    ##  5 PASIR RIS             3920.
    ##  6 JURONG WEST           3928.
    ##  7 BUKIT PANJANG         4016.
    ##  8 BUKIT BATOK           4126.
    ##  9 HOUGANG               4182.
    ## 10 SENGKANG              4341.
    ## # … with 16 more rows
