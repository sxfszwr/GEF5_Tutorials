# GEF5_Tutorials

## Introduction

**Graphical Editing Framework**

The Eclipse Graphical Editing Framework (GEF) provides Eclipse-integrated end-user tools in terms of a Graphviz authoring (DOT editor, DOT Graph view) and a word cloud rendering environment (Tag Cloud view), as well as framework components (Common, Geometry, FX, MVC, Graph, Layout, Zest, DOT, and Cloudio) to create rich graphical JavaFX- and SWT-based client applications, Eclipse-integrated or standalone.


## Install

- Install jdk8
- Download Eclipse Oxygen
- Install e(fx)clipse-IDE-PDE from `Menu->Help->Install New Software` by [http://download.eclipse.org/releases/oxygen](http://download.eclipse.org/releases/oxygen)

## Set up target definition containing GEF

- Create a file and name it `gef-integration.target` , then paste the following content into it.


~~~
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<?pde version="3.8"?><target name="gef-integration" sequenceNumber="1">
<locations>
  <location includeAllPlatforms="false" includeConfigurePhase="true" includeMode="planner" includeSource="true" type="InstallableUnit">
    <unit id="org.eclipse.xtext.sdk.feature.group" version="2.10.0.v201605250459"/>
    <unit id="org.eclipse.fx.runtime.min.feature.feature.group" version="2.4.0.201605100504"/>
    <unit id="org.eclipse.emf.sdk.feature.group" version="2.12.0.v20160526-0356"/>
    <unit id="org.eclipse.sdk.ide" version="4.6.0.I20160606-1100"/>
    <repository location="http://download.eclipse.org/releases/neon"/>
  </location>
  <location includeAllPlatforms="false" includeConfigurePhase="true" includeMode="planner" includeSource="true" type="InstallableUnit">
    <unit id="org.eclipse.gef.common.sdk.feature.group" version="0.0.0"/>
    <unit id="org.eclipse.gef.geometry.sdk.feature.group" version="0.0.0"/>
    <unit id="org.eclipse.gef.fx.sdk.feature.group" version="0.0.0"/>
    <unit id="org.eclipse.gef.mvc.sdk.feature.group" version="0.0.0"/>
    <unit id="org.eclipse.gef.mvc.examples.source.feature.group" version="0.0.0"/>
    <unit id="org.eclipse.gef.layout.sdk.feature.group" version="0.0.0"/>
    <unit id="org.eclipse.gef.graph.sdk.feature.group" version="0.0.0"/>
    <unit id="org.eclipse.gef.zest.sdk.feature.group" version="0.0.0"/>
    <unit id="org.eclipse.gef.zest.examples.source.feature.group" version="0.0.0"/>
    <unit id="org.eclipse.gef.dot.sdk.feature.group" version="0.0.0"/>
    <unit id="org.eclipse.gef.cloudio.sdk.feature.group" version="0.0.0"/>
    <repository location="http://download.eclipse.org/tools/gef/updates/integration"/>
  </location>
</locations>
</target>
~~~
	
- Open gef-integration.target with target editor, make sure it loaded all unit.

- set it as active target platform

## Run the demo 

- Clone the code from `https://github.com/eclipse/gef.git`

- Copy the following project into your workspace

	- org.eclipse.gef.cloudio.examples.ui
	- org.eclipse.gef.dot.examples
	- org.eclipse.gef.fx.examples
	- org.eclipse.gef.fx.examples.swt
	- org.eclipse.gef.geometry.examples
	- org.eclipse.gef.graph.examples
	- org.eclipse.gef.layout.examples
	- org.eclipse.gef.zest.examples
	- org.eclipse.gef.zest.examples.jface 


