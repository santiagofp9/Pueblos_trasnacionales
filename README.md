# Pueblos_trasnacionales
Which towns near Madrid are populated with foreign communities?

My project for this week is to gather the base data for my final project.
The idea is to generate a map of Comunidad de Madrid, based on the birthplace of every registered habitant.
This concept will render a map of foreign communities in Madrid.



Expected outcome and minimum viable product:

-Associates every population point (Municipio) with a given coordinate, matching with Google Maps. 
-Groups population points (Municipios) into geoeconomic areas inside Madrid. 
-Returns demographic data and population composition by birthplace. 
-Has clear documentation on how to insert data to cross-reference it with this database. 
-Escalates relationships based on coordinates.


Next steps:

-Cross-reference the original database with PIB data. 
-Extends the dataset back to 1985, when the nationality records start. 
-Show the economic evolution of high-density foreign population centres. 
-Correlates economic growth with migration.


Escalable outcome:

This will be a tool to cross-reference fine-grained data. Possible use on social research (education, governance or culture).


Potential risks:

Identifying ghetto structures, in the worst-case scenario, could help to exacerbate them. An interview with an expert in the field would be necessary to adjust the code.



Steps:

1. The base source shows the population of every town, by birth country. Instituto de Estadística. Padrón continuo 2021. 350 population points, 208 birthplaces. 2.4MB
1.1 This base file can already be shaped into a database since it has several layers. Also population percentages will be calculated.

2. The next step will be to enrich the base table with PIB (Producto Interno Bruto). Instituto de Estadística offers data only from 2009 and back. Grouped by agriculture, industry and services.
2.1.A new source will be needed for fine-grained PIB in Comunidad de Madrid, El País and other media that make regular use of this data must research their source.

3. Coordinates indexed in Google Maps will be scrapped for every population point (350).
3.1 GMaps has a territorial delimitation called 'place' it is better defined object than a coordinate (includes coordinate). Also the zip code must be extracted.


BIBLIO:

More than numbers: How migration data can deliver real-life benefits for migrants and governments.
(International Organization for Migration, Jan 2018)
https://www.mckinsey.com/industries/public-and-social-sector/our-insights/how-migration-data-can-deliver-real-life-benefits-for-migrants-and-governments

Corridors and characteristics; Effects on GDP, productivity, and employment; Better integration outcomes.
"People on the move", McKinsey report, 2016, PDF
'https://www.mckinsey.com/~/media/mckinsey/industries/public%20and%20social%20sector/our%20insights/global%20migrations%20impact%20and%20opportunity/mgi-people-on-the-move-full-report.pdf'
