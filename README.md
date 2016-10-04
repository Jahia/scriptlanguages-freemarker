# scriptlanguages-freemarker

A Jahia Digital Experience Manager (DX) module that provides FreeMarker scripting language support. This module 
should mostly be considered as a proof-of-concept. It is not recommended to use this code in a production environment.
For more information about Jahia DX, please go to: https://www.jahia.com/platform/digital-experience-manager

## Features
- Makes it possible to use FreeMarker as a scripting languages for Jahia views
- All standard Jahia variables are exposed as FreeMarker variables, you can display node contents, etc.

## Requirements
- Jahia 7.2.0.0 or more recent
- Maven 3.0+ for module compilation
- JDK 7+

## Usage

1. Compile the whole project using : mvn clean install
2. Deploy the core/target/scriptlanguages-freemarker*.jar and examples/target/scriptlanguages-freemarker-example*.jar modules
3. In Edit mode, add a Basic Content -> freeMarkerNode content node, and enter a value for the freeMarkerText property.
The value of this property will be displayed by the node template written in FreeMarker.

## Example template

You will find an example template in the following directory : examples/src/main/resources/jnt_freeMarkerNode/html/freeMarkerNode.fm