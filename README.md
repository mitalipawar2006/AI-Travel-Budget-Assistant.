# ✈️ AI Travel Budget Assistant

An AI-powered travel planning assistant built using **Activepieces, Generative AI, JavaScript, Google Forms, and the Frankfurter Exchange Rate API**. It helps travellers understand their budgets in their destination's currency and generates a personalized travel budget report delivered directly to their email.

## 📌 Project Overview

Planning a trip involves managing expenses such as flights, accommodation, food, transportation, and activities. Travellers may also struggle to understand how much their money is worth in a foreign currency.

The AI Travel Budget Assistant simplifies this process by collecting travel details through a Google Form, converting the budget into the destination currency, and using Generative AI to create a practical travel budget report.

## 🎯 Objectives

- Automate travel budget calculations.
- Convert currencies using exchange rate data.
- Generate personalized travel budget reports using AI.
- Suggest daily spending limits and expense allocations.
- Provide practical money-saving tips.
- Deliver the generated report directly to the user's email.

## 🛠️ Technologies Used

- **Activepieces:** Workflow automation and integration.
- **Google Forms:** Collects travel information from users.
- **Google Sheets:** Stores form responses.
- **Google Apps Script:** Sends form submissions to the Activepieces webhook.
- **JavaScript:** Processes travel details and calculates currency conversions.
- **Frankfurter API:** Retrieves exchange rate information.
- **Generative AI:** Generates personalized travel budget reports.
- **Gmail:** Sends the final report to the traveller.

## ⚙️ How It Works

The project follows an automated workflow:

1. **User Input:** The traveller submits a Google Form containing the destination, total budget, budget currency, destination currency, trip duration, and email address.

2. **Form Integration:** Google Apps Script sends the submitted information to the Activepieces webhook.

3. **Currency Conversion:** The JavaScript code retrieves the exchange rate through the Frankfurter API and calculates the converted budget and estimated daily budget.

4. **AI Report Generation:** The AI step generates a personalized report containing the budget summary, expense allocations, exchange rate details, daily spending allowance, and money-saving tips.

5. **Email Delivery:** The completed travel budget report is sent to the traveller through Gmail.

## ✨ Key Features

- Automated collection of travel details.
- Currency conversion between supported currencies.
- Automatic calculation of the converted budget.
- Estimated daily spending allowance.
- AI-generated travel budget reports.
- Suggested expense allocations for flights, accommodation, food, local transport, attractions, shopping, and emergencies.
- Destination-specific money-saving tips.
- Automatic delivery of reports through email.

## 💰 Travel Expense Categories

The generated report provides suggested budget allocations for:

- Return flights or intercity travel
- Accommodation
- Food and drinks
- Local transportation
- Attractions and activities
- Shopping and miscellaneous expenses
- Emergency reserve

The allocations are estimates and should be adjusted after checking actual prices. The total allocations should not exceed the traveller's available budget.

## 🔄 Workflow Architecture

Google Forms  
↓  
Google Sheets and Google Apps Script  
↓  
Activepieces Webhook  
↓  
JavaScript Code Step  
↓  
Frankfurter Exchange Rate API  
↓  
Generative AI Report Generation  
↓  
Gmail  
↓  
Travel Budget Report Delivered to User

## 🚀 Setup and Configuration

To run this project:

1. Create a Google Form with the required travel information fields.
2. Link the form to a Google Sheets response spreadsheet.
3. Configure Google Apps Script to send form submissions to the Activepieces webhook.
4. Import the exported workflow JSON into Activepieces.
5. Configure the webhook trigger and reconnect the required AI and Gmail connections.
6. Ensure the JavaScript code step is configured to retrieve exchange rates and calculate the converted budget.
7. Test the workflow with sample travel details.
8. Publish the workflow and submit a new Google Form response to test the complete process.

**Note:** The exported workflow may require connection setup and webhook configuration before it can run successfully in another account.

## 📊 Example Output

For a traveller planning a trip to Rome, the assistant can generate a report containing:

- Destination and trip duration
- Original and converted budget
- Exchange rate and rate date
- Estimated daily spending allowance
- Suggested expense allocations
- Money-saving tips
- Travel budgeting reminders

The report is automatically delivered to the email address provided by the traveller.

## ⚠️ Limitations

- Exchange rates may change over time.
- The report provides suggested budget allocations, not guaranteed travel prices.
- Actual flight, accommodation, and activity costs depend on booking dates, preferences, and availability.
- Travellers should verify actual prices before making reservations.
- The workflow requires correctly configured connections and a working internet connection.

## 🔮 Future Enhancements

- Integration with live flight and hotel price APIs.
- Destination recommendations based on the available budget.
- Multi-destination itinerary planning.
- Interactive travel expense tracking.
- WhatsApp notifications.
- PDF report generation.
- Improved recommendations based on traveller preferences.

## 👩‍💻 Author

**Mitali Pawar**

Project: AI Travel Budget Assistant

## 📄 License

This project is intended for educational and demonstration purposes. A license can be added if the project is distributed for reuse.
