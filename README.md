# Kata kesh
Stargate themed katas focusing on microservices.

## About
Right now, this readme is the placeholder. The plan is to create katas that allow one or more people to solve them in one or two hours and for them to be relatively technology agnostic.

There will be some dependencies that need to be run, I'm currently not sure of the best way to do this, it's probably going to be a container that you'll have to run in your container runtime of choice.

## Katas

### Welcome to Cheyenne Mountain Dr Jackson
Establish comms with the Gate and control dialling via gate remote procedure calls (gRPC), 
Requires: Gate service to be created
Challenge: talking gRPC to gate service

### Cheyenne Mountain Operations Centre
We need mountain operations to be able to control it so our DHD needs to be able to be controlled but the mountain operations only speaks REST.
Requires: Operations service to be created
Challenge: to make previous client a service in its own right

### Gate Discovery
We need to start finding valid gate addresses, the only way is to dial (first 10 unique addresses fail, next 3 pass so it's not a brute force challenge)
Requires: message queue and publisher?
Challenge: to read messages off a queue..?

### Power Drain
Add in a rate limiting challenge to stop the gate from drawing too much power. Can maybe put a limit of 20 per minute and therefore the previous kata when run longer would start throwing errors.
Requires: service that can repeatedly send requests to Gate service
Challenge: to rate limit

## Contribute

Myself and Icepuma over on Rawkode's [Discord](https://discord.com/invite/rawkode) were throwing around ideas about this in the Help channel, feel free to join the server and discuss any ways to make this better, be it lore, challenges or dependencies. 
