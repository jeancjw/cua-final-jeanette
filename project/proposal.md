CUA Project Proposal: An exploratory study of Airbnb rentals in
Singapore
================
Jeanette Choong
3/5/2020

## 1\. Introduction

Airbnb, which puts together bed and breakfast listings from all over the
world on an online platform, has been increasingly popular amongst
tourists who prefer to stay in a local home at their destinations. The
growth of Airbnb also sees homeowners taking the opportunity to create
homely spaces, which are sometimes themed to fit various traveller
preferences, giving them an alternative lodging experience that is
unique from the monotonous hotel scene (Fig 1). The proliferation of
Airbnbs around the world have also put a spolight on its negative
effects on communities, neighbourhoods, housing market and the hotel
industry.

<div class="figure">

<img src="/Users/jeancjw/Documents/SUTD/MUSPP/02.522 Urban Data & Methods II CUA/cua-jeanette-c/images/airbnb.png" alt="Fig 1. Airbnb listing in Singapore (Source: Airbnb, 2020)" width="932" />

<p class="caption">

Fig 1. Airbnb listing in Singapore (Source: Airbnb, 2020)

</p>

</div>

The Airbnb scene in Singapore is especially different because of the
strict laws and regulations that surround short-term rentals in the
city-state. Unlike other countries, the passing of these rental laws has
steered the nation’s Airbnb market away from conventional tourist
groups. However, as of February 2020, there are 8047 Airbnb listings in
Singapore (Inside Airbnb, 2020), which is surprising, considering the
laws that surround rentals. These include both public and private
housing. Therefore, this project aims take on an exploratory approach to
gaining insight about the Airbnb rentals in Singapore and why they still
exist despite strict laws.

## 2\. Literature Review

This section discusses literature regarding the effects that Airbnb
rentals have had on cities, and the ways in which Singapore’s policies
have been shaped to curb the negative effects on short-term rentals like
Airbnbs.

### 2.1 Positive effects of Airbnbs for travellers

According to Airbnb (2020a), the rise in listings has given millions the
experience of living like a local, which 91% of travellers today want to
do. This had led Airbnb listings to focus on neighbouhoods outside the
usual tourist districts. This has also boosted the income of hosts, of
whom 52% are from low to middle income families (Airbnb, 2020a).
However, this also causes problems for cities.

### 2.2 Negative effects on neighbourhoods and society

A study conducted on Barcelona’s old town revealed that 9.6% of homes
were listed on Airbnb, and within its Gothic Quarter, this percentage
was 16.8% (Cocola-Gant, 2016). Cocola-Gant (2016) argues that the
prevelance of holiday rentals such as Airbnbs is one of the key reasons
for urban gentrification and displacement of residents by tourists.

In an attempt to upkeep mutli-racial integration and inclusivity in
Singapore, the government has rolled out the HDB Ethnic Integration
Policy, which provides an ethnic quota for public housing estates. While
the efficacy of the quota is debatable, the impact on society and
individual neighbourhoods could be a strong enough reason for the
government to come up with these short-term rental laws, so as to upkeep
a sense of identity amongst Singaporeans in these neighbourhoods.

### 2.3 Negative effects on traditional tourist lodging

Unsurprisingly, there has also been an effect on the hotel industry. The
“Airbnb effect”, threatens hotel revenues as a result of cheaper and
sometimes, better-quality Airbnb listings (Gerdeman, 2015). Gerdeman
(2015) revelead that this effect was particularly significant in cities
where hotels had limited vacancies during peak periods, as the surge in
Airbnb listings forced hotels to draw down their prices despite
eventually being fully-booked.

### 2.4 Singapore’s Laws on Short-term Rentals

While there are no laws against tourists staying in Airbnbs per se, the
laws governing short-term rentals/accommodation restrict tourists from
seeking Airbnbs as a potential accommodation when visiting Singapore.
The Singapore government has imposed these laws to ensure safety and
privacy, and minimise disturbances in residential areas, which may come
about when residential areas are frequented by tourists (URA, 2020).

Under the 2017 Planning Act, private housing have to be rented out for a
minimum of three consecutive months (or 90 days) to the same person
(SSO, 2020), while HDB flats require a minimum rental period of six
months (180 days) under the Housing and Development Act. Additionally,
flat owners must obtain approval from HDB for such rentals (HDB, 2020).

## 3\. Research Question(s) & Hypotheses

While Airbnb (2020a) claims to have provided benefits to travellers and
hosts around the world, discussions by various literature seem to focus
on the negative effects on neighbourhoods, housing market and especially
the hotel industry (Coldwell, 2017; Xie & Kwok, 2017; Ioannides,
Röslmaier & Van de Zee, 2018; Nieuwland & van Melik, 2018). This
phenomenon, also known as the “Airbnb effect” has taken a toll on
revenue for the hotel industry as a result of intense competition
(Gerdeman, 2018). Perhaps, this is why Singapore has so many strict laws
on short-term rentals.

This leads us to the research question: Why are there still so many
Airbnb listings in Singapore despite these strict laws?

In this context, here are the hypotheses of this study:

1.  Many home owners may be flouting the rules.

2.  The Airbnb market in Singapore targets Singaporeans, permanent
    residents, and long-term stayers with appropriate passes.

3.  Most listings would be located in neighbourhoods where there are
    fewer HDB flats as it is more challenging for owners to meet the
    180-day minimum stay.

Some guiding questions include: 1. How risky is it for a tourist to stay
in an Airbnb accommodation? 2. Which listings are likely violating the
laws on short-term rentals in Singapore? 3. How much does it cost to
rent a place from Airbnb in Singapore? 4. Where are most listings
located at? 5. How does the availability vary with the type of listing?

## 4\. Data Sources

Data on the Airbnb rentals in Singapore is publicly available through
the Inside Airbnb website at
`http://insideairbnb.com/get-the-data.html`. Datasets are updated
monthly, but for the sake of this project, I will be using data as of 27
February 2020.

There are three main components to the dataset:

  - `listings`: Provides detailed listings data for Singapore, including
    location, price, minimum length of stay, number of reviews, hosts
    and listing ID.
  - `reviews`: Provides date and details of reviews and reviewer.
  - `calendar`: Provides details of bookings across a year for each
    listing.

Additionally, I may use the following datasets to enhance my data
analyses and visualisations:

  - Planning area data from OneMap APIs
  - Open data from HDB on data.gov.sg regarding rental demand, approvals
    and prices

The data is generally clean, but will require some degree of
manipulation in the analysis process.

## 5\. Research Approach

This study will take on a quantitative approach to finding out why
Airbnbs still thrive in Singapore in spite of the strict laws.

First, I aim to display the listings visually, in order to identify
where most listings are located at, by planning area or neighbourhood.

Second, I will analyse the number of reviews, and the minimum length of
stay stipulated by hosts, which can be used as a proxy for hosts who are
violating the short-term rental laws. This could also be used to assess
the risk a tourist faces in choosing to book these Airbnb listings.

Finally, I will find out the cost of renting Airbnbs, and the
distribution across locations and time. Seasonal peaks in costs could
correspond to peaks in tourism, and locations may relate to popular
tourist destinations. The presence of these peaks may indicate a higher
likelihood of hosts flouting the rules - though not certainly.
Furthermore, prices would give us a sense of what the demand is like,
and therefore address why Airbnbs continue to exist in Singapore.

## 6\. Preliminary Data Analyses & Visualisation

``` r
library(tidyverse)
library(here)
library(httr)
library(mapedit)
library(mapview)
library(sf)
library(skimr)
library(lubridate)
library(forcats)
library(tmap)
```

``` r
calendar_feb20 <- read_csv(here::here("projdata/calendar-feb20.csv"))
```

    ## Parsed with column specification:
    ## cols(
    ##   listing_id = col_double(),
    ##   date = col_date(format = ""),
    ##   available = col_logical(),
    ##   price = col_character(),
    ##   adjusted_price = col_character(),
    ##   minimum_nights = col_double(),
    ##   maximum_nights = col_double()
    ## )

``` r
listings <- read_csv(here::here("projdata/listings-feb20.csv"))
```

    ## Parsed with column specification:
    ## cols(
    ##   id = col_double(),
    ##   name = col_character(),
    ##   host_id = col_double(),
    ##   host_name = col_character(),
    ##   neighbourhood_group = col_character(),
    ##   neighbourhood = col_character(),
    ##   latitude = col_double(),
    ##   longitude = col_double(),
    ##   room_type = col_character(),
    ##   price = col_double(),
    ##   minimum_nights = col_double(),
    ##   number_of_reviews = col_double(),
    ##   last_review = col_date(format = ""),
    ##   reviews_per_month = col_double(),
    ##   calculated_host_listings_count = col_double(),
    ##   availability_365 = col_double()
    ## )

``` r
listings_sf <- st_as_sf(listings, coords = c("longitude", "latitude"), crs = 4326) %>%
  st_transform(3414)
# convert coordinates to be the same as those used on OneMap
```

### 6.1 No. of listings in the past year

``` r
# values based on number of observations from previous months' listings
listings_time <- tribble(
  ~month, ~total_listings,
  "feb20", 8047,
  "jan20", 7857,
  "dec19", 8000,
  "nov19", 7857,
  "oct19", 7794,
  "sep19", 7675,
  "aug19", 7907,
  "jul19", 8033,
  "jun19", 8293,
  "may19", 8325,
  "apr19", 8090,
  "mar19", 7975
)

month_order <- c(
  "mar19", "apr19", "may19", "jun19", "jul19", "aug19", "sep19", "oct19", "nov19",
  "dec19", "jan20", "feb20"
)

listings_time %>%
  mutate(month = ordered(month, levels = month_order)) %>%
  ggplot(aes(x = month, y = total_listings)) + geom_col(color = "grey", fill = "paleturquoise3") + geom_text(aes(label = total_listings), vjust = -0.5, size = 3) + labs(y = "Total listings")
```

![](proposal_files/figure-gfm/unnamed-chunk-4-1.png)<!-- -->

While the number of listings looks quite stable over the past year,
slight peaks can be observed during months that coincide with higher
tourist volumes, such as May to June, and from December to February.
Notably, listing numbers increased in February 2020 amidst the covid-19
situation, which is interesting considering the hotel industry has
suffered a backlash due to reduced tourist traffic. Perhaps, these
listings target long-term stayers more than tourists.

Instead, if we look a tthe number of reviews over the years, it is
apparent that the Airbnb scene has gained popularity over the years.

### 6.2 Reviews over time

``` r
reviews_feb20 <- read_csv(here::here("projdata/reviews-feb20.csv"))
```

    ## Parsed with column specification:
    ## cols(
    ##   listing_id = col_double(),
    ##   id = col_double(),
    ##   date = col_date(format = ""),
    ##   reviewer_id = col_double(),
    ##   reviewer_name = col_character(),
    ##   comments = col_character()
    ## )

``` r
reviews_feb20 %>%
  ggplot() + geom_bar(aes(date)) + labs(y = "number of reviews") + theme_light()
```

![](proposal_files/figure-gfm/unnamed-chunk-6-1.png)<!-- -->

The number of reviews seem to have increased over time.

``` r
listings %>%
  group_by(neighbourhood) %>%
  count() %>%
  arrange(-(n)) %>% 
  head(10) %>% 
  kable()
```

| neighbourhood |    n |
| :------------ | ---: |
| Kallang       | 1168 |
| Geylang       |  976 |
| Novena        |  594 |
| Rochor        |  587 |
| Downtown Core |  518 |
| Outram        |  483 |
| Bukit Merah   |  385 |
| River Valley  |  355 |
| Bedok         |  343 |
| Queenstown    |  298 |

### 6.3 Listings by region

``` r
listings_sf %>%
  group_by(neighbourhood_group) %>%
  count()
```

    ## Simple feature collection with 5 features and 2 fields
    ## geometry type:  MULTIPOINT
    ## dimension:      XY
    ## bbox:           xmin: 7215.566 ymin: 25166.35 xmax: 43591.65 ymax: 48466.72
    ## epsg (SRID):    3414
    ## proj4string:    +proj=tmerc +lat_0=1.366666666666667 +lon_0=103.8333333333333 +k=1 +x_0=28001.642 +y_0=38744.572 +ellps=WGS84 +units=m +no_defs
    ## # A tibble: 5 x 3
    ## # Groups:   neighbourhood_group [5]
    ##   neighbourhood_gro…     n                                              geometry
    ## * <chr>              <int>                                      <MULTIPOINT [m]>
    ## 1 Central Region      6582 ((20066.19 30441.98), (20167.47 30480.68), (20199.74…
    ## 2 East Region          468 ((35692.49 35206.65), (36017.47 34665.95), (36049.74…
    ## 3 North Region         206 ((15354.78 44677.6), (19559.1 43038.7), (19648.18 44…
    ## 4 North-East Region    308 ((27345.79 39523.39), (27365.82 39556.56), (27488.24…
    ## 5 West Region          483 ((7215.566 33484.57), (9320.744 43116.64), (10737.87…

``` r
# Planning region .shp file was downloaded from https://geo.data.gov.sg/mp14-region-web-pl/2014/12/05/shp/mp14-region-web-pl.zip

pln_area_polyg <- read_sf(here::here("projdata/pln_boundary/MP14_REGION_WEB_PL.shp"))
```

``` r
# visually
tmap_mode("view")
```

    ## tmap mode set to interactive viewing

``` r
tm_shape(listings_sf) +
  tm_dots(col = "neighbourhood_group", size = 0.08) + tm_shape(pln_area_polyg) + tm_text("REGION_N")
```

    ## Warning: The shape pln_area_polyg is invalid. See sf::st_is_valid

![](proposal_files/figure-gfm/unnamed-chunk-10-1.png)<!-- -->

### 6.4 Prices in Central Region

``` r
listings_sf %>%
  filter(neighbourhood != "Tuas") %>% 
  group_by(neighbourhood) %>%
  summarise(mean_price = mean(price)) %>%
  ggplot(aes(x = neighbourhood, y = mean_price)) + geom_col(color = "grey", fill = "paleturquoise3") + theme(axis.text.x = element_text(angle = 90, hjust = 1))
```

![](proposal_files/figure-gfm/unnamed-chunk-11-1.png)<!-- --> Southern
islands has the highest mean price for Airbnbs in the Central region,
followed by Marina South and Orchard.

### 6.5 Minimum number of nights

``` r
below_90 <- listings_sf %>%
  select(id, host_name, neighbourhood, neighbourhood_group, minimum_nights, geometry) %>%
  filter(minimum_nights < 90)
```

A quick glance at the number of listings that are potentially violating
the law (less than 90-day minimum stay), shown by coloured
dots.

``` r
tm_shape(listings_sf) + tm_dots(col = "black", size = 0.01) + tm_shape(below_90) + tm_dots(col = "neighbourhood_group", alpha = 0.4, size = 0.01)
```

![](proposal_files/figure-gfm/unnamed-chunk-13-1.png)<!-- -->

### 6.6 Top host

The top host has 340 listings.

``` r
listings %>% 
  group_by(host_id) %>% 
  select(host_id, host_name, calculated_host_listings_count) %>% 
  arrange(desc(calculated_host_listings_count))
```

    ## # A tibble: 8,047 x 3
    ## # Groups:   host_id [2,561]
    ##     host_id host_name calculated_host_listings_count
    ##       <dbl> <chr>                              <dbl>
    ##  1 66406177 Jay                                  340
    ##  2 66406177 Jay                                  340
    ##  3 66406177 Jay                                  340
    ##  4 66406177 Jay                                  340
    ##  5 66406177 Jay                                  340
    ##  6 66406177 Jay                                  340
    ##  7 66406177 Jay                                  340
    ##  8 66406177 Jay                                  340
    ##  9 66406177 Jay                                  340
    ## 10 66406177 Jay                                  340
    ## # … with 8,037 more rows

## 7\. References

Airbnb. (2020). Modern & Stylish Bedroom + Mins walk to MRT. Retrieved
from
<https://www.airbnb.com.sg/rooms/40407434?location=Singapore&source_impression_id=p3_1583722438_qW7vmjnKD5rs%2FxAM>

Airbnb. (2020a). The Economic Impacts of Home Sharing in cities around
the world. Retrieved from <https://www.airbnb.com/economic-impact>

Cocola-Gant, A. (2016). Holiday Rentals: The New Gentrification
Battlefront. Sociological Research Online, 21. <doi:10.5153/sro.4071>

Coldwell, W. (2017). First Venice and Barcelona: now anti-tourism
marches spread across Europe. The Guardian, 10, 2017. Retrieved from
<https://www.theguardian.com/travel/2017/aug/10/anti-tourism-marches-spread-across-europe-venice-barcelona>

Gerdeman, D. (2018). The Airbnb Effect: Cheaper Rooms for Travellers,
Less Revenue for Hotels. Forbes. Retrieved from
<https://www.forbes.com/sites/hbsworkingknowledge/2018/02/27/the-airbnb-effect-cheaper-rooms-for-travelers-less-revenue-for-hotels/#7f757cc3d672>

Inside Airbnb. (2020). Get the Data. Retrieved from
<http://insideairbnb.com/get-the-data.html>

Nieuwland, S., & van Melik, R. (2018). Regulating Airbnb: how cities
deal with perceived negative externalities of short-term rentals.
Current Issues in Tourism, 1-15. <doi:10.1080/13683500.2018.1504899>

Ioannides, D., Röslmaier, M., & van der Zee, E. (2019). Airbnb as an
instigator of ‘tourism bubble’ expansion in Utrecht’s Lombok
neighbourhood. Tourism Geographies, 21(5), 822-840.
<doi:10.1080/14616688.2018.1454505>

Singapore Statutes Online. (2020, 30 June 2017). Planning Act (Amendment
of Fourth Schedule) Order 2017. Retrieved from
<https://sso.agc.gov.sg/Act/PA1998>

Urban Redevelopment Authority. (2020). Short-Term Accommodation.
Retrieved from
<https://www.ura.gov.sg/Corporate/Property/Residential/Short-Term-Accommodation>

Xie, K. L., & Kwok, L. (2017). The effects of Airbnb’s price positioning
on hotel performance. International Journal of Hospitality Management,
67, 174-184. <doi:https://doi.org/10.1016/j.ijhm.2017.08.011>
