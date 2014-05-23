Simple Tycho Sample
====================

Main purpose of this project is to explore how to properly build a simple 
eclipse update site containing a simple plugin and associated source code.

Run the build as follows:

     mvn -Pe43 clean install
     
After a succesful build the update site (p2 repository) will be in:

     hello.world.site/target/repository
     
The project consists of the following:
   - pom.xml: parent pom in the root of the tree. Configures needed bits (i.e. tycho and its plugin-sources and feature-sources plugins)
   - hello.world.plugin simple plugin. 
   - hello.world.feature: feature containing the plugin
   - hello.world.site: site containing the feature. 
