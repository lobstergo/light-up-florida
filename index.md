# LIGHT UP FLORIDA
## Challenge Statement 4: Power Consumption

<iframe width="800" height="450" src="https://www.youtube.com/embed/_dOer8_41tc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Introduction
The sunny state of Florida, located in the southeastern part of the United States, is a dream place where people yearn for the good life. Introducing new sources of energy to improve Florida's energy generation and build a better, healthier, greener Florida is the challenge we need to address.

## Problems
Today, Florida's energy problems cannot be ignored. It uses more energy per capita than all but two states, and it is the fourth-largest energy consumer, consuming almost eight times as much energy as it produces. Its serious power consumption issue also leads to high CO2 emissions.  Florida ranked **fourth in terms of Natural Gas Consumption** while ranked **third for total C02 Emissions**.

Florida's high CO2 Emission is mainly due to the **unfit resource structure**, in other words, it has too many high-carbon sources but will have few renewable sources. The non-renewable resources Florida had,  such as natural gas, coal, and petroleum provided approximately 80.3% of Florida's energy and generated a significant amount of CO2 in the process of use. Additionally, its high-carbon source has an energy consumption of 3626.1 Trillion Btu whereas renewable energy with only 617.5 trillion Btu energy consumption. 

## Target
It is no exaggeration to say that optimizing Florida's energy structure and reducing carbon emissions are imminent. Using renewable energy instead of a high-carbon source is a more intuitive way, two methods could be used to reach this target, which could be concluded as **more renewable energy and less traditional energy**. 

![IMG 1 Renewable Energy Consumption](https://user-images.githubusercontent.com/94873300/144022838-43f147cb-3cea-4f7d-8d31-c2cee5ee6613.png)

## Solution
Among all the renewable energy, **solar** is a renewable energy source that we should concentrate on. Based on the data from State Energy Data Systems, the four most commonly used renewable resources in Florida are solar, biomass, hydropower, and wind energy. Each has its own advantages and disadvantages. It is worth noticing that although most renewable energy sources emit much less carbon than high-carbon sources, biomass and hydropower are two renewable energy sources with relatively high carbon emissions, solar and wind, on the other hand, are both environmentally friendly. However, given the fact that Florida's flat terrain and not reaching wind speeds with an annual average of 6.5 meters per second at a height of 80 meters. **Solar energy is the most suitable for Florida with its advantages like limitless source, low carbon emission, decreasing installation costs, and no noise in comparison**. 

On the other side, Florida wants to **reduce its use of coal and natural gas**. First, natural gas and coal emit large amounts of carbon dioxide; second, Florida imports almost all of its coal and natural gas, which can significantly increase costs; and third, natural gas is inevitably harmful to groundwater when it is used to generate energy. 

To conclude, traditional energy needs to be replaced by the use of solar energy. However, that brings up another problem: How? This could also be divided into two parts, build solar power plants and reduce the use of traditional energy.

## How It Works
The techniques of **Machine learning** were used in this study.

### Modeling
In order to predict suitable locations for solar power plants in Florida, we decided to build a machine learning model.

In our previous research, we found that the main factors that determine whether a solar power station can be built are light conditions, geographical location, and local population and economic conditions. So first we collected location data for five states with similar lighting conditions and recorded their zip-code, longitude, latitude, population, average income, and the number of solar power plants.

![IMG 2 Data Frame](https://user-images.githubusercontent.com/94873300/144023708-fc35e2ec-fc57-4434-9c16-a4ab73821167.jpeg)

Among the 2,694 locations, 182 have solar stations.

![IMG 3 Bool Have Solar Station](https://user-images.githubusercontent.com/94873300/144023928-06492a3e-6b04-4104-a822-0ef1eeec9316.jpeg)

In our visualization analysis, we can also see the influence of these attributes on whether a solar station can be built.

![IMG 4 Influence Visual](https://user-images.githubusercontent.com/94873300/144024101-46062c1d-1185-4310-9829-9c8b30beb030.jpeg)

First, we try to establish a linear regression model. We use 70 percent of the data for training and 30 percent for testing. The accuracy of the model is obtained.

![IMG 5 Linear Regression](https://user-images.githubusercontent.com/94873300/144024446-38a5a5c0-9272-43b5-b08c-bec05c40bd5e.jpeg)
![IMG 6 Import Metrics](https://user-images.githubusercontent.com/94873300/144024464-d9ed2e27-cd4f-4ee0-ba32-a2781a34332d.jpeg)

We imported data from Florida and made projections.

![IMG 7 df_F](https://user-images.githubusercontent.com/94873300/144024733-b8e2624f-a471-453b-901a-59079c27558e.jpeg)

In view of the limitations of linear regression, we decided to build another logistic regression model.

![IMG 8 Split](https://user-images.githubusercontent.com/94873300/144024907-b65d9a4b-f313-4457-90d4-692646e136b4.jpeg)

![IMG 9 Accuracy](https://user-images.githubusercontent.com/94873300/144024916-ad63ba76-0e5d-4074-93a0-e515a80b9603.jpeg)

And using data from Florida to predict. The two models output their respective prediction results.

### Result
After combining the results of the two models, we came up with 18 suitable locations for solar power stations. 12 of the locations already had solar power stations, so our machine learning models eventually found 6 suitable locations for solar power stations. The theoretical optimal **6 zip codes** for building PV plants are 33012, 33063, 33064, 33065, 33311, and 33313.

![IMG 10 Predictions Result](https://user-images.githubusercontent.com/94873300/144025326-c78403de-f4ff-408b-92d9-93414ae773e2.jpeg)

### Feasibility Analysis
After conducting a feasibility analysis, there are certain risks associated with the construction of solar power plants. First, the construction of solar power plants have high infrastructure construction costs; second, its related core technology is still in the research and development stage and is not advanced enough; finally, due to environmental constraints such as no solar energy at night, or in cool, cloudy climates, in these environments does not generate enough solar energy. But there are also significant benefits to building solar power plants. First, low environmental management costs or import costs; second, great potential for future technological development; and third, no greenhouse gas emissions. Except for the expense aspect, the other two advantages of solar stations can make up for the shortfalls.

According to our calculations, the fixed cost of building a typical size PV plant is equivalent to the sum of 3.68 years' carbon treatment costs for a conventional power generation facility at the same capacity, which means the **cost** of building a PV plant **can be covered within 4 years**.

![IMG 11 Feasibility Analysis](https://user-images.githubusercontent.com/94873300/144026987-e4d8979a-aec4-439e-b13c-303bbb091297.jpeg)

## Conclusions & Look Forward
To sum up, through machine learning we were able to find the theoretical **optimal locations** for **future solar stations**. Simultaneously, we are able to illustrate the **economic** and **environmental benefits** and viability of this strategy through thorough calculations. Therefore, it has been demonstrated in numerous ways that expanding the use of solar energy rather than traditional energy is a viable strategy to improve Florida's energy generation and thus develop a better, healthier, and greener future for Florida.

We advocate the development of **Energy Storage Tech** that lets the electricity generated in the day be used at night. Less traditional energy will be used, and Florida will eventually reach **carbon neutrality**.


------------------------------------

## Works Cited
“Florida Municipal Electric Association.” Florida Municipal Electric Association, 2021, 
	www.flpublicpower.com.

“Florida - State Energy Profile Overview - U.S. Energy Information Administration (EIA).” EIA 
	Beta, 2019, www.eia.gov/state/?sid=FL.

Gerardi, Jeff. “Power Plant Construction: How Much Does It Cost?” ProEst, 24 Feb. 2021, 
	proest.com/construction/cost-estimates/power-plants.

"Orlando City Energy Project Impact Study (2015-2030)." City of Orlando, 2015, 
https://www.orlando.gov/files/sharedassets/public/initiatives/bewes/orlando-bewes-impact-study.pdf

“Orlando, FL Electricity Rates.” Electricity Local, 2021, 
	www.electricitylocal.com/states/florida/orlando.

“Sunrise and Sunset Times in Orlando.” Timeanddate, 2021, 
	www.timeanddate.com/sun/usa/orlando.

“The True Cost of Reducing Greenhouse Gas Emissions – IMF F&D | DECEMBER 2019.” 
	International Monetary Fund, 2019, 
www.imf.org/external/pubs/ft/fandd/2019/12/the-true-cost-of-reducing-greenhouse-gas-emissions-gillingham.htm.

“U.S. Data.” NSRDB, 2021, nsrdb.nrel.gov/about/u-s-data.html.

“United States - U.S. Energy Information Administration (EIA).” EIA Beta, 2019, 
	www.eia.gov/beta/states/states/fl/overview.

“Zip Codes with the Highest Median Household Income in Florida | Zip Atlas.” Copyright 2011 
	ZipAtlas.Com, 2011, zipatlas.com/us/fl/zip-code-comparison/median-household-income. 
	htm.


------------------------------------------------
