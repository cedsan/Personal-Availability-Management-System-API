# Personal AvailabilityManagement System API

## Terminology

**Observable** - User that provides availability information for __*Obervers*__ users to subscribe to.

**Observer** - User that subscribes to the availability information provided by __*Observables*__ users.


## Motivation

The Personal Availability Management System API service originated from the need for college students to easily know of a professor's availability. Nowadays, obtaining this information would require for a student to email/message the professor asking if she/he is available.

This interaction used to obtain a professor's availability, although being simple, it's repetitive and may require for the professor to have to share the same information multiple times in a single availability window.

The purpose of this service is to take advantage of today's client devices (computer or mobile devices) notification capabilities to automate the propagation of the availability information to subscribed __*Observers*__.


## Description

This Personal Availability Management System API service allows for an __*Observable*__ user to configure multiple time windows of availability during a week.

Users interested in the __*Observable*__'s availability can subscribe to her/him.

By using the service, the process to automate the provision of availability information is: 
1. The __*Observable*__ configures time windows of availability for a week, at a given location (for example, the college institution where the professor teaches);

2. A companion mobile client application, making use of mobile devices geolocation services, detects when the __*Observable*__ enters the configured location, and if in an availability window, updates the __*Observable*__ *Available* state in the service;

3. When receiving a request to make the __*Observable*__ available, the service notifies all __*Observers*__ subscribed to the __*Observable*__.


This project was implemented in the context of my bachelor's final project at [ISEL - Instituto Superior de Engenharia de Lisboa](https://www.isel.pt/). 





