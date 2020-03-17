[![Board Status](https://dfatkulbayanova.visualstudio.com/0132b0f0-36b9-415c-aac8-1b0cbda27828/3fbae06a-b5db-41e3-9597-9b25d1a7ae79/_apis/work/boardbadge/442adf50-a345-4237-9dd7-94e83186a22d)](https://dfatkulbayanova.visualstudio.com/0132b0f0-36b9-415c-aac8-1b0cbda27828/_boards/board/t/3fbae06a-b5db-41e3-9597-9b25d1a7ae79/Microsoft.RequirementCategory)
# Project Name

The DevOps open hack event is designed to foster learning via implementing DevOps practices with a series of challenges.

## Architecture

The application used for this event is a heavily modified and recreated version of the original [My Driving application](https://github.com/Azure-Samples/MyDriving).

The team environment consists of the following:

* Azure Kubernetes Service (AKS) cluster which has four APIs deployed:

  * POI (Trip Points of Interest) - CRUD API written in .Net Core 2 for points of interest on trips
  * Trips - CRUD open API written in golang 1.11 for trips connected to the client application
  * UserProfile - CRUD open API written in Node.JS for the users of the client application
    > Note:PATCH/POST operations not functional
  * User-Java - API written in Java with POST and PATCH routes plus swagger docs routes for the users of the client application.
* Mobile Apps - for iOS and Android which will display driving trip data

## Getting Started

To understand each of the components above in more detail, please visit the readme files inside the root folder of each corresponding part of the application.

### Prerequisites

It is useful but not required to have a basic knowledge of the following topics:

* Kubernetes
* Azure DevOps (formally VSTS) or Jenkins

## Resources

The provisioning of this environment for proctors can be found in the [DevOps Openhack Proctor](https://github.com/Azure-Samples/openhack-devops-proctor) Github repository.
