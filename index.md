# LIGHT UP FLORIDA
## Challenge Statement 4: Power Consumption

<p align = "center">
<iframe width="800" height="450" src="https://www.youtube.com/embed/sRneDVWu3Hw" title="YouTube video player" frameborder="0" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

## Introduction
The sunny state of Florida, located in the southeastern part of the United States, is a dream place where people yearn for the good life. Introducing new sources of energy to improve Florida's energy generation and build a better, healthier, greener Florida is the challenge we need to address.

## Problems
Today, Florida's energy problems cannot be ignored. It uses more energy per capita than all but two states, and it is the fourth-largest energy consumer, consuming almost eight times as much energy as it produces. Its serious power consumption issue also leads to high CO2 emissions.  Florida ranked fourth in terms of Natural Gas Consumption while ranked third for total C02 Emissions.

Florida's high CO2 Emission is mainly due to the unfit resource structure, in other words, it has too many high-carbon sources but will have few renewable sources. The non-renewable resources Florida had,  such as natural gas, coal, and petroleum provided approximately 80.3% of Florida's energy and generated a significant amount of CO2 in the process of use. Additionally, its high-carbon source has an energy consumption of 3626.1 Trillion Btu whereas renewable energy with only 617.5 trillion Btu energy consumption. 

## Target
It is no exaggeration to say that optimizing Florida's energy structure and reducing carbon emissions are imminent. Using renewable energy instead of a high-carbon source is a more intuitive way, two methods could be used to reach this target, which could be concluded as **more renewable energy and less traditional energy**. 

![IMG 1 Renewable Energy Consumption](https://user-images.githubusercontent.com/94873300/144022838-43f147cb-3cea-4f7d-8d31-c2cee5ee6613.png)

## Solution
Among all the renewable energy, solar is a renewable energy source that we should concentrate on. Based on the data from State Energy Data Systems, the four most commonly used renewable resources in Florida are solar, biomass, hydropower, and wind energy. Each has its own advantages and disadvantages. It is worth noticing that although most renewable energy sources emit much less carbon than high-carbon sources, biomass and hydropower are two renewable energy sources with relatively high carbon emissions, solar and wind, on the other hand, are both environmentally friendly. However, given the fact that Florida's flat terrain and not reaching wind speeds with an annual average of 6.5 meters per second at a height of 80 meters. Solar energy is the most suitable for Florida with its advantages like limitless source, low carbon emission, decreasing installation costs, and no noise in comparison. 

On the other side, Florida wants to reduce its use of coal and natural gas. First, natural gas and coal emit large amounts of carbon dioxide; second, Florida imports almost all of its coal and natural gas, which can significantly increase costs; and third, natural gas is inevitably harmful to groundwater when it is used to generate energy. 

To conclude, traditional energy needs to be replaced by the use of solar energy. However, that brings up another problem: How? This could also be divided into two parts, build solar power plants and reduce the use of traditional energy.

## How It Works
The techniques of Machine learning were used in this study.

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
After combining the results of the two models, we came up with 18 suitable locations for solar power stations. 12 of the locations already had solar power stations, so our machine learning models eventually found 6 suitable locations for solar power stations.

![IMG 10 Predictions Result](https://user-images.githubusercontent.com/94873300/144025326-c78403de-f4ff-408b-92d9-93414ae773e2.jpeg)









------------------------------------------------
You can use the [editor on GitHub](https://github.com/lobstergo/light-up-florida/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/lobstergo/light-up-florida/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
