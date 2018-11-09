# Content-Bundle for Office Locations
❗️ This bundle is no longer needed for map.apps line 4 apps. The domain bundle mechanism can be used to add content via bundles. It is a map.apps core functionality. See administration guide for further details. ❗️

This example configuration of a content bundle adds a thematic map service to the map, extends the search and registers simple thematic data dialogs.

"Load the bundle for production sites in the app" should not just mean  that the data is loaded into the map, and the object attributes can be visualised in a pop-up by clicking on something. If apps are designed to provide optimal business data support, it should mean much more: Provision of specific, business-focussed dialogues that represent the semantics of the data with uncompromised search and query definitions, additional specialist tools and widgets, security, data sources and more. These aspects have been offered by map.apps since version 1.0, and appreciated by customers. As of now, the first bundle is available that wraps up all of these aspects so they can be added to an app with a single step! In this way, customers can add a bundle repository to content bundles so that apps can be extended, according to the use case, by a click. The app is then injected with the necessary pieces needed. So now, specialist editors can add the "production sites" content to an app, just like they add a standard widget today, but including all of the above. map.apps and the creator of the bundle takes care of the details.

For this function we now offer a first implementation for free download. The example configuration of Content Bundles bound to the locations of Esri companies in the map, extends the search and registers simple thematic data dialog for the businesses. All this can of course be copied and reconfigured as required.

Development Guide
------------------
### Define the mapapps remote base
Before you can run the project you have to define the mapapps.remote.base property in the pom.xml-file:
`<mapapps.remote.base>http://%YOURSERVER%/ct-mapapps-webapp-%VERSION%</mapapps.remote.base>`

##### Other methods to to define the mapapps.remote.base property.
1. Goal parameters
`mvn install -Dmapapps.remote.base=http://%YOURSERVER%/ct-mapapps-webapp-%VERSION%`

2. Build properties
Change the mapapps.remote.base in the build.properties file and run:
`mvn install -Denv=dev -Dlocal.configfile=%ABSOLUTEPATHTOPROJECTROOT%/build.properties`

