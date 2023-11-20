# Currency Converter UI

This Currency Converter UI allows users to convert amounts from one currency to another. The application is built using ReactJS v18 with TypeScript.

## Table of Contents

- [Functional Requirements](#functional-requirements)
- [Mock API for Exchange Rates](#mock-api-for-exchange-rates)
- [Unit Testing](#unit-testing)
- [Bonus Requirements](#bonus-requirements)
- [Folder Structure](#folder-structure)
- [How to Run](#how-to-run)
- [Testing](#testing)
- [Follow-up Interview](#follow-up-interview)

## Functional Requirements

1. **Currency Conversion UI:**

   Your UI should have the following elements:

   - **Source Currency Dropdown:** A dropdown menu on the left side of the screen labeled "Source Currency". This is where users select the currency they want to convert from.
   - **Target Currency Dropdown:** A dropdown menu on the right, parallel to the source currency dropdown, labeled "Target Currency". Users select the currency they want to convert to.
   - **Amount Input Field:** A field below the currency dropdowns where users can input the amount they want to convert. This field should be clearly labeled, such as "Enter Amount".
   - **Convert Button:** A button below the amount input field, labeled "Convert". Clicking this button will trigger the conversion process.
   - **Converted Amount Display:** An area or field below the convert button where the converted amount is displayed. This could be labeled as "Converted Amount" or "Result".

   Please do input validation. Also, please display clear, descriptive error messages (if any) in toast notifications.

2. **Mock API for Exchange Rates:**

   You need to create a mock API against which the UI will make HTTP calls to extract the exchange rates. Use axios's mock adapter or mock service worker to implement this.

   The mock API should support conversions between the following currency pairs: USD, INR, EUR. It should simulate responses for invalid input, unsupported currencies, transient network errors, rate limits, delayed responses, etc.

3. **Unit Testing:**

   Write unit tests for the conversion logic. Tests must cover various scenarios, including edge cases & negative cases. Use any testing framework of your choice (e.g., Jest, react-testing-library, etc).

## Bonus Requirements

The UI should be responsive and render correctly on various form factors: desktops, mobile devices, tablets.

## Folder Structure

```plaintext
currency-converter-app/
|-- src/
|   |-- components/
|   |   |-- CurrencyConverter/
|   |   |   |-- CurrencyConverter.tsx
|   |   |   |-- CurrencyConverter.test.tsx
|   |-- services/
|   |   |-- api.ts
|-- utils/
|   |   |-- validation.ts
|-- README.md
|-- package.json
