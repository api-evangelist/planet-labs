<!-- fetched 2026-10-14 from https://developers.planet.com/docs/basemaps/tile-services/ by sweep-geospatial.py; text extracted from the provider's own page -->

Tile Services | Planet Documentation Skip to main content 
 Platform Develop Data Guides Help Status 
 Community 
 University 
 Help Center 
 Publications Database 
 Pricing 
 More Platform 
 Develop 
 Data 
 Guides 
 Help 
 Status 
 Support Center 
 Community 
 University 
 Publications Database 
 Pricing 
 Ask AI 
 Search 
 Free Trial 
 Developer Overview 
 APIs 
 Analytics 
 Asynchronous Processing 
 Basemaps 
 Batch Processing 
 Batch Statistical 
 Bring Your Own COG 
 Catalog 
 Data 
 Destinations 
 Features 
 Orders 
 Processing 
 Quota 
 Reports 
 Statistical 
 Subscriptions 
 Tasking 
 Tiles 
 WMTS 
 XYZ 
 Third-Party Data Import 
 Zarr Import 
 Authentication 
 Errors 
 Rate Limiting 
 SDKs and Developer Resources 
 Evalscripts 
 Changelog 
 Develop 
 APIs 
 Tiles 
 On this page 
 Copy for LLM View as Markdown 
 Tile Services
 The API Tile Service and Mosaic Tile Service make it easy to visualize Planet imagery in desktop or web mapping applications that support either the XYZ or the WMTS protocol. Planet tile services provide a way for web developers and GIS analysts to interact with, and derive value from Planet imagery without additional image processing.
 Authentication ​ 
 A valid Planet account is required to access either of the tile services (XYZ or WMTS). Authenticate by providing a valid api_key as a query parameter to all tile requests.
 info
 You must be authenticated to use Planet tile services. If you do not have the correct permissions, the tile request results in a 404 error. To be properly authenticated, provide a valid api_key as a query parameter in all tile requests.
 API Key Security ​ 
 Your Planet API key grants you access to Planet products. Like other credentials, you must take precautions to ensure it stays secure.
 If you use your API key to load tiles for web map applications, additional steps are required to keep the key secure. Do not commit your API key to code repositories, do not store or use the API key in code used by the public or your users (For example, frontend web applications), and make sure that requests made by web applications you create do not expose the API key while fetching tiles. We recommend that you use your API keys only within secure environments that you control. For security purposes, applications running on end users' systems must not fetch tiles directly from Planet using your API key. This includes web applications that users access with their browser.
 Contact Planet Support to obtain a new key or if your API key is shared or exposed.
 Tile Service URLs ​ 
 The Planet tile services provide tiles by using the following domains:
 https://tiles0.planet.com 
 https://tiles1.planet.com 
 https://tiles2.planet.com 
 https://tiles3.planet.com 
 Load more tiles concurrently in web browsers by using multiple subdomains. Libraries such as OpenLayers and Leaflet provide the ability to access all subdomains by using the proper string patterns.
 note
 The Tile Services API does not have rate limits. For general rate limiting information, see the rate limiting page.
 API Tile Service ​ 
 The API Tile Service acts as an extension to the Planet API by visually listing the Planet assets that are available in the item archive as tiles. The imagery returned by the tile service is a compressed version of the high-quality visual asset, making it easy to incorporate into any supporting client. Currently, only clients using the XYZ tile protocol are supported.
 API Tile Service Request Structure 
 https://tiles{0-3}.planet.com/data/v1/{item_type}/{item_id}/{z}/{x}/{y}.png?api_key={pl-api-key} 
 API Tile Service Request in Python with Basic HTTP Authentication 
 Python
 import os 
 # import os module to access environmental modules 
 import requests 
 from requests . auth import HTTPBasicAuth 
 # import helper functions to make Basic request to Planet API 
 PLANET_API_KEY = os . getenv ( "PL_API_KEY" ) 
 # Setup the API Key from the `PL_API_KEY` environment variable 
 BASE_URL = "https://tiles{0-3}.planet.com/data/v1/{item_type}/{item_id}/{z}/{x}/{y}.png" 
 if PLANET_API_KEY is None : 
 PLANET_API_KEY = "12345" 
 # pass in your API key 
 auth = HTTPBasicAuth ( PLANET_API_KEY , "" ) 
 # HTTPBasicAuth() wants a username & password; you can pass an empty string for the password 
 res = requests . get ( url = BASE_URL , auth = auth ) 
 print ( res . status_code ) 
 # make a request to Tile Services API and test the response 
 Parameter | Value | 
 item_type | Item type of the item to view. | 
 item_id | Item id of the item to view. | 
 z | Tile zoom level. | 
 x | Tile row in the grid. | 
 y | Tile column in the grid. | 
 The following example is a complete URL for a tile request for the PSScene item with an id of 20161221_024131_0e19 :
 https://tiles1.planet.com/data/v1/PSScene/20161221_024131_0e19/14/12915/8124.png?api_key={pl-api-key} 
 Mosaic Tile Service ​ 
 The Mosaic tile service provides access to tiles for weekly or monthly, color corrected global mosaics. The Mosaic tile service works with any client that supports the XYZ or the WMTS protocol.
 Details on Planet specifications are available in PlanetScope Mosaics Product Specifications .
 Dynamically Rendering False-Color Indices ​ 
 The PlanetScope Surface Reflectance Mosaic products are also available in false-color visualizations to support a wider range of analysis. Currently the following seven band combinations and indices are available via Tile Service:
 Red-Green-Blue (RGB)
 Color-infrared (CIR)
 Normalized Difference Vegetation Index (NDVI)
 Normalized Difference Water Index (NDWI)
 Visual Atmosphere Resistance Index (VARI)
 Modified Soil-adjusted Vegetation Index (MSAVI2)
 Modified Triangular Vegetation Index (MTVI2)
 Triangular Greenness Index (TGI)
 note
 False-color indices and band math visualizations are available only on Surface Reflectance Mosaics.
 Remote Sensing Indices ​ 
 Index | Formula | Legend | URL Parameters | 
 NDVI | i r − r i r + r \frac{ir - r}{ir + r} i r + r i r − r ​ | | ?proc=ndvi | 
 NDWI | g − i r g + i r \frac{g - ir}{g + ir} g + i r g − i r ​ | | ?proc=ndwi | 
 MSAVI2 | 2 ∗ i r + 1 − ( 2 ∗ i r + 1 ) 2 − 8 ( i r − r ) 2 \frac{2 * ir + 1 - \sqrt{(2 * ir + 1)^2 - 8(ir - r)}}{2} 2 2 ∗ i r + 1 − ( 2 ∗ i r + 1 ) 2 − 8 ( i r − r ) ​ ​ | | ?proc=msavi2 | 
 MTVI2 | 1.5 ∗ ( 1.2 ∗ ( i r − g ) − 2.5 ∗ ( r − g ) ( 2 ∗ i r + 1 ) 2 − ( 6 ∗ i r − 5 ∗ r ) − .5 \frac{1.5 * ( 1.2 * (ir - g) - 2.5 * (r - g)}{\sqrt{(2 * ir + 1) ^ 2 - (6 * ir -5 * \sqrt{r})} - .5} ( 2 ∗ i r + 1 ) 2 − ( 6 ∗ i r − 5 ∗ r ​ ) ​ − .5 1.5 ∗ ( 1.2 ∗ ( i r − g ) − 2.5 ∗ ( r − g ) ​ | | ?proc=mtvi2 | 
 VARI | g − r g + r − b \frac{g - r}{g + r - b} g + r − b g − r ​ | | ?proc=vari | 
 TGI | ( 120 ∗ ( r − b ) ) − ( 190 ∗ ( r − g ) ) 2 \frac{(120 * (r - b)) - (190 * (r - g))}{2} 2 ( 120 ∗ ( r − b )) − ( 190 ∗ ( r − g )) ​ | | ?proc=tgi | 
 Additional Resources 
 🎓 Planet University
 Dive deeper into Planet services with guides and tutorials
 Tile Services in ArcGIS Online
 Explore Using Planet Tile Services in ArcGIS Online
 Was this helpful? 
 Last updated on Apr 24, 2026 
 Previous
 API Reference
 Next
 WMTS
 Authentication 
 API Key Security 
 Tile Service URLs 
 API Tile Service 
 Mosaic Tile Service 
 Dynamically Rendering False-Color Indices 
 Remote Sensing Indices 
 Company
 Visit Planet.com 
 Talk to Sales 
 Get Started 
 News
 Blog 
 Sign Up for News 
 Product Updates 
 Support
 Planet Community 
 Planet University 
 Planet Publications 
 Help Center 
 © 2026 Planet Labs PBC All rights reserved. 
 Privacy Policy | California Privacy Notice | Your Privacy Choices | Terms of Use | Cookie Notice | Sitemap
