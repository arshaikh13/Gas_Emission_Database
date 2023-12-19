Greenhouse Gas Emission Database Description

Purpose: This SQL database meticulously captures and organizes crucial data related to greenhouse gas emissions, providing a comprehensive insight into 
the environmental impact of various countries and industries. The database consists of four interconnected tables: Country, Gases, Industry, 
and Greenhouse_Output, each playing a pivotal role in highlighting the intricate relationships between population, emissions, and contributing sectors.

Table Descriptions:

Country:Records vital information about countries, including CountryName, Population, and TotalArea_sq_mi.
Primary key: CountryName.

Gases:Contains details about different greenhouse gases, such as GasName, Percentage, and Effect.
Primary key: GasName.

Industry: Focuses on industries and their contributions to greenhouse gas emissions.
Includes IndustryName, PercentContribution, and a foreign key GasName referencing the Gases table.
Primary key: IndustryName.

Greenhouse_Output: Provides insights into the global output percentages of greenhouse gases by countries and industries.
Features GreenhouseID, CountryName, IndustryName, and PercentGlobalOutput.
Primary key: GreenhouseID.
Foreign keys: CountryName references Country(CountryName), and IndustryName references Industry(IndustryName).

Key Queries:

Viewing: Lists all countries and their populations from the database.

Filtering Countries:Identifies countries ending in "sia" and displays their populations.

Industry Filter: Selects countries with a 'K' in their name, where the main polluting industry is electricity/heat.

Gas Count:Determines the total number of gases in the database.

Global Output:Presents the percent global output of each country with a population exceeding 100,




