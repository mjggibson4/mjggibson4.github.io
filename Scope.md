# Scope Document

## Purpose
This document outlines what was aimed to be achieved within Practical 1 of the module: Programming for Geographical Information Analysts: Core Skills (WUN). This scope includes any extra functionality which has been included.

## Initial Scope of Project
The overarching aim of this project was to produce an agent based model that interacted with an input enivironment. In this model only one type of agent would be present. These agents would have the ability to move randomly around the enviroment, nibble away at it and share resources. This model should have a GUI allowing user inputs and the results projected within an animated figure.

## Extended Scope
This initial scope was extended for the final project that was submitted. This basic agent based model was extended into a simple model of predator prey dynamics between two defined agents classes. These agents classes were defined as being that of sheep and wolves. In order for this model to work, a defined set of rules were constructed by which agents must follow:

###Rules
* Both sheep are wolf agents will be moved randomly
* The expection to this is at boundary of the enivronment's domain. In these scenarios an agents movement should be restricted such that the agent remain in the domain.
* Sheep nibble the enviroment 10 units at a time. This resource is place in a store
* If 10 units are not present in a sheep's location, the sheep consumes the resource that is available.
* Sheep have the ability to share resources with sheep that lie within a user defined distance
* Sheep reproduce at a threshold value set by the user
* On reproduction, the store of a sheep will be reset to 0
* Wolf agents do not consume the environment
* Wolf agents consume any sheep that lie adjacent to their location and increase their store by 1
* Wolf agents will reproduce at a threshold value set by the user

## GUI
To reflect this extended scope, the GUI should be updated to allow the user to have more control of the model and it's output. The following parameters within the model are to be defined by the user:

* Number of Sheep - The initial number of sheep agents to be placed in the model
* Number of Wolves - The initial number of wolf agents to be placed in the model
* Neighbourhood - The distance at which sheep are allowed to share resources
* Number of Iterations - The number of iterations for which the model will run
* Wolf Threshold - The number of sheep needed to be eaten by a wolf in order for it to reproduce
* Sheep Threshold - The amount of units of environment needed to be consumed by a sheep in order for it to reproduce
