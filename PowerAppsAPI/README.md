# Without Pre-Built Connectors in Power Apps

This app demonstrates how to integrate external APIs into Power Apps without relying on pre-built connectors. It uses a **Power Automate Flow** with the HTTP connector to interact with the **Recipe API** endpoint from [API Ninja](https://api-ninjas.com/).

## Overview

The **Without Pre-Built Connectors** app showcases:
- How to set up a Power Automate flow for custom API integration.
- Using the HTTP connector in Power Automate to connect with the Recipe API.
- Fetching and displaying data from API Ninja's Recipe API in Power Apps.

## Key Features

- **Power Automate Integration**:
  - The app calls a Power Automate flow to handle API requests.
  - HTTP connector in Power Automate is configured to communicate with the Recipe API.

- **Dynamic Recipe Search**:
  - Users can search for recipes by ingredient or cuisine.
  - The app displays results in a gallery format for easy browsing.

- **Error Handling**:
  - Includes basic error handling to manage cases where the API returns no results or fails.

## How to Use This App

1. **Download the App**:
   - Download the `.msapp` file: [Without Pre-Built Connectors.msapp](./Without%20Pre-Built%20Connectors.msapp).

2. **Obtain an API Key**:
   - To test this app, you must obtain your own API key from [API Ninja](https://api-ninjas.com/).
   - Sign up for an account, navigate to the Recipe API page, and copy your API key.

3. **Set Up the Power Automate Flow**:
   - Create a Power Automate flow using the **HTTP connector**.
   - Configure the flow as follows:
     - **Method**: `GET`
     - **Endpoint**: [API Ninja's Recipe API](https://api-ninjas.com/api/recipes)
     - **Authentication**: Add your API key in the headers.

   Example headers:
   ```json
   {
       "X-Api-Key": "YOUR_API_KEY"
   }
   ```

4. **Connect the Flow to Power Apps**:
   - Import the Power Automate flow into Power Apps.
   - Bind the flow to a button or gallery to fetch data dynamically.

5. **Test the App**:
   - Run the app in Power Apps Studio.
   - Enter an ingredient or cuisine to search for recipes.
   - Observe the gallery updating with data fetched from the Recipe API.

## Resources

- **Video Tutorial**: [How YOU Can Make API Calls in Power Apps WITHOUT Pre-Built Connectors](https://www.youtube.com/watch?v=F2xAhKpS-Mc)
- **API Ninja Documentation**: [Recipe API](https://api-ninjas.com/api/recipes)
- **Power Automate Documentation**: [HTTP Connector](https://learn.microsoft.com/en-us/power-automate/connectors/standardhttp/)

## Screenshots

| Feature                     | Preview                                |
|-----------------------------|----------------------------------------|
| Recipe Search by Ingredient | *(Add screenshot here)*               |
| Displaying Recipe Results   | *(Add screenshot here)*               |
