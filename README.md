# WTF
Quick and dirty change of algorithm from the original:
- "put on the server with smallest amount of players"
to:
- "put on a random server except for the most occupied one"

Good for testing, but still suffers a crash if one of the servers dies.
So fix before running it in production. :D

Made for MultiPaper, can load balance 20 players per second easily.


# VelocityLoadBalancer
A simple plugin to balance player counts on a Velocity proxy.

## Installation
  * Download the latest release from the [releases tab](https://github.com/bhopahk/VelocityLoadBalancer/releases).
  * Put the jar in your Velocity plugins folder
  * Restart Velocity
  
## Configuration
LoadBalancer does not have a configuration file and uses the fallback servers defined inside the Velocity server to decide which server the player will be connected to.  

## Building LoadBalancer
The releases tab will be updated for notable changes to the plugin, however if you would like the have the bleeding edge version you can build the plugin yourself.
  * Pull the repository using whichever method you are most comfortable
  * Run the `build` gradle task using a local gradle distribution or the included gradle wrapper.
