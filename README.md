# Assist a Purchase

Philips has many monitoring solutions, as [seen here](https://www.philips.co.in/healthcare/solutions/patient-monitoring/continuous-patient-monitoring-systems).

This project assists in selecting and delivering the right solution. It serves both the customer as well as Philips personnel.

It has two segments:

1. The API, which is consumed by GUI and non-GUI clients.
GUI-clients are for standalone use of this product.
Non-GUI clients are other systems that need to integrate with this product.
1. The GUI, which is one client of the API

## [Segment 1] Web API

The web-service must respond with answers to questions in a stateless manner. This is a technique for scaling your solution. The server’s resource-requirements are greatly simplified when it doesn’t need to keep track of every client’s question-sequence.

Every interaction with the chat-bot interface shall be designed to accept the context and respond with the next question and its choices.
The web-service shall offer interfaces for configuration: Loading the device database, adding new models and removing obsolete ones.
It shall also offer an interface to alert subscribers when a user selects a model. A possible subscriber could be the sales department of the region, for example.
Optionally, the web-service needs to be extended to other languages as well.
