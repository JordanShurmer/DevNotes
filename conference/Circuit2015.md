[TOC]

Circuit Conference 2015
===================

Keynote
----------

----------

Accessibility
---------------

----------

AEM Apps/Cordova
----------------------
* Content Sync - creates a zip file of changes made after a given time!
 
----------

Adobe Apps Component Development
---------------------------------------------

----------

Devs the New Author (dialog story telling)
--------------------------------------------------
The dialog is a powerful way we, as developers, have to communicate directly to the content authors. It should tell a story.

* Nested components, rather than a listing dialog thing. (e.g. each image in a photo gallery shows up as it's own component on the edit page!
	* Inherit from parses?
	* Include a parsys.
* Maven component plugin.
* https://itHub.com/Citytechnic/cq-component-maven-plugin
* Jordan.miller@icfi.com

Modern Front End Build Tools in AEM
---------------------------------------------
Slidedeck: http://slides.com/benwestrate/deck/live

###Why?
1. Dev Speed
2. Code Organization
3. Reusability
4. Nodejs (gives you build tools, file system API, etc....)

###In AEM
* Not a great workflow currently. 
* Maven + Node = Awesome
* Maven Front End Plugin
	* Allows us to pull node in to the mvn project
	* The full power of node inside the arm project
		* gulp/grunt/build tools
		* js lint/compile
		* less/sass
	* (Not installing nodejs on the computer)
	* com.github.eirslett frontend-maven-plugin
	* iron-fe node project from icf
		* Auto-generate the maven xml files and blueprint directories for the Maven Front End stuffages
* gulp-slang for watching/updating

-----

Maximize the pore of OSGi in AEM
-----------------------------------------
(David Bosschaert)
### OSGi promises
* OSGi aries
* Javascript-style promises, can be used with Java 5 or later
	* Asynchronous chaining
	* Very simply programming model
* Promises can be used outside of the OSGi framework

###OSGI Services intro
* Services are Java Objects (POJOs)
	* registered by Bundles
	* consumed by Bundles
* "SOA inside the JVM"
* Services looked up by type and/or custom filter
	* "I want a service that implements org.acme.Payment where location=US"
	* One or many returned
* Dynamic! Services can be updated without taking down the consumer
	* OSGI Service Consumer react to dynamism

### Async Services

### Notes
* @interface annotation for component configuration! (maven bundle plugin)
* Declarative Services
* OSGi Subsystems (instead of AEM Packages for the bundles)
	* Zip file with .esa extension
	* feature
	* application
	* composite
	* ESA Maven Plugin
* OSGi Enterprise R6 (http://www.osgi.org/Download/Release6)


10 Things Apache Sling Can Do...
---------------------------------------
History
* Code donation to Apache in 2007
	* OSGi implementations
	* Tooling
	* Sling Framework
* ~40 committers
* Highly Modular
* ~15 releases per month
* Platform for Adobe AEM
* Used by various companies

1. Sustainable through modularity
	* Modules from the start
	* Very stable client API (+7 years)
	* Extensions
	* The Power of OSGi
2. 