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
