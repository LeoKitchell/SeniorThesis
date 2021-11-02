# Exploring Gentrification Using Airbnb Data

This repository is a living log of my senior thesis research. It is very much a work in progress; please excuse the mess. 

## Research Question

Throughout this process, my guiding research question will be: *can neighborhood residents see gentrification in action and can this awareness be translated into a useful quantitative tool for researchers.*


## Motivation & Background

Gentrification is a hot topic in literature and the public discourse. It is also something I'm woefully unknowledgeable about. I'm undertaking this research project in order to deepen my understanding and potentially contribute to the quantitative understanding of the subject.

Gentrification is generally understood as a process of change whereby neighborhoods which have been historically under-capitalized experience an influx of new residents with high social capital. This demographic change corresponds with an increase in investment in the neighborhood, generally transforming the housing stock and character of the neighborhood, while also displacing the original lower income residents of the neighborhood. Each of the three pillars of change (demographic, housing and retail stock, and cultural character) have characteristics which make quantifying their change difficult, and which consequently limits scholarship and effective policy intervention. 

One of the principle data challenges is that detailed demographic data is infrequently collected, so researchers and policymakers are constantly fettered by data from the Census or the 5 year American Community Survey. This lag means that research must be conducted on sparse time series, limiting the research's power, while on the policy side the lag makes early identification of gentrification difficult, and dynamic monitoring impossible. Changes in the physical neighborhood real-estate composition are generally the easiest to detect, as home prices, building permits, and other measures of investment operate on shorter lag. The final pillar of change is also the most difficult to quantify. While the arrival of craft coffee shops, whole foods, and street art may be easily visible signs of cultural change for residents of a gentrifying neighborhood, this local knowledge does not get translated into traditional data sets. However, new data sources may solve some of these challenges.

Today, more complicated and less structured data are becoming available to researchers with a lag of weeks or months, rather than years. While some of these data are also found in traditional datasets, there also exist new, less structured features which can be used to better understand neighborhoods and their residents. In this project I plan to use listing data on Airbnbs in major US cities to determine neighborhood features associated with gentrification. While these data may be able to pick up demographic changes in neighborhoods, I believe they will provide the most use in quantifying cultural change. This quantification will be a function of both structured features, such as the density of listings and their prices, and unstructured features, namely the text descriptions of Airbnb listings and their neighborhoods. *If the markers of cultural change are indeed visible to residents, the text description of a given Airbnb and its neighborhood should reflect that change.*

## Preliminary Literature Review

### Well Understood Portions of Gentrification

Suburbs have become less appealing to high wage workers as their leisure time has diminished. This has increased demand for urban housing stock, reversing a 1980s trend of suburbanization, and causing housing proximate to central business districts to balloon in price (Edlund 2015). At the same time, decades of "urban revitalization" projects are coming to fruition **(citation needed)**, further increasing metropolitan neighborhood home prices. Consumer tastes are also changing **(citation needed)** as new workers demand to be in culutural cities (potential research: are young tech workers making different housing choices than young, rich workers from the 50s-90s). Crime rates in cities have also fallen dramatically since the 90s, further bolstering home prices in urban areas **(citation needed)**.


### Different Specfification of Gentrification
Glaeser(2020) defines gentrifying areas as "places with high initial poverty, relative to the city as a whole, and high rent growth." They also use a secondary specification which inclues an "increasing education and increasing share of white residents" as measures of gentrification. 
Jain (2021) 
Slater(2006;2009), Newman and Wyly (2006), Davidson and Lees (2005) argue that displacement is "a constituent element of gentrification" (Goetz). In this view, displacement must be included in the gentrification specification to properly measure its effects. However, as Goetz et. al. write, "empiracally establishing the degree of displacement is one of the most difficult aspects of gentrification research...Even when data exist that might highlight one form of displamcement, typically most of then other forms of displacement remain largely hidden."

### My Specification of Gentrification
Following in the footsteps of other empirical studies of gentrification, the unit of analysis will be census tract, using ACS 5 year data. A further examination using block groups may be conducted, time permitting, but we hypothesize that insufficient density of Airbnb's will rend the predictive power of the textual data minimal in all but the most dense tracts. To reflect the multi-stage nature of gentrification, our analysis will first identify tracts that are gentrifiable.
Like Bostic and Martin (2003), Freeman (2005), and McKinnesh et al. (2010 **CHECK**), getntrifiable tracks will be defined as those with a median income less than 50% of the median income of the metropolitan statistical area in which they are contained.  

### Independent Variables

Based off of Jain (2021), but instead of reducing the dimensionality of the text data in LDA and Doc2Vec we keep the full variation of text by using a random forest regression methodlogy to test the significance od diffferent words in the review. 

### Additional Methodological Ideas
We also plan on testing the affect of location scores and rentals that have a minimum of 30 days or more per stay. It is our hope that renters who stay longer than 30 days develop a deeper understanding of the neighborhood, which can be better translated to text, and experience the neighborhood ammenities in the same way that a traditional resident of the neighborhood would, rather than a tourist. 

## Running List of Potential Flaws

Airbnb descriptions are targeted toward a userbase which is predominately composed of high income members. These users may also be young. The descriptions may therefore misrepresent the actual characteristics of the neighborhood in favor of those which are attractive to the target audience. An audience which shares many of the same characteristics of gentrifiers. 


