# Credit Offers API Reference Application Code

Credit Offers is a card acquisition service that provides prequalified credit offer listings based on end customer provided information. Affiliates are able to provide these offers directly without need of a web redirect.  If a prequalified offer is not available, a default offer is returned by us.

## Software Requirements Including version
This is version 1.0 of the Credit Offers API Reference Application Code. For software requirements, see Build/Install Instructions below.

This reference app illustrates the use of the Credit Offers API to collect customer information and retrieve a list of targeted product offers for display. If you encounter any issues using this reference code, please submit them in the form of GitHub issues.

## Build/Install Instructions

### config.js
You can configure your clientID and clientSecret in credit-offers/config.js. In addition, if you change the default port for the mock API, you also need to update this file.

### Start the mock API
From the project root:  
`cd credit-offers_mock_api`  
`npm install`  
`npm start`

### Start the app
From the project root:  
`cd credit-offers`  
`npm install`  
`npm start`

### Try it out

Navigate to http://localhost:3000.  You will see a simple page with a button to launch a customer info modal.  Enter some fake customer data (at least the minimum required fields) and submit the form.  

This will submit a request to the Credit Offers endpoint and redirect the user to a page displaying the offers.

### Viewing more details

To get a deeper look at the messages being passed, start the app with the following command `DEBUG=credit-offers:* NODE_DEBUG=request npm start`.  This will activate detailed debug logging to the console, showing the details of the request to the API and the response received.

## Architecture

## Roadmap
This reference app code is intended as a starting place for developers who want to use the Credit Offers API. As such, it will be updated with new functionality only when the Credit Offers API is updated with new functionality.

## Contribution Guidelines
We encourage any contributions that align with the intent of this project and add more functionality or languages that other developers can make use of. To contribute to the project, please submit a PR for our review. Before contributing any source code, familiarize yourself with the Apache License 2.0 (license.md), which controls the licensing for this project.
