# Currency Converter Web App

## Overview
This is a simple **Currency Converter Web App** built with **React.js**. It allows users to convert currencies using real-time exchange rates fetched from the **FawazAhmed Currency API**. The app features an intuitive UI and supports swapping currencies instantly.

## Features
- Convert currencies dynamically
- Fetch real-time exchange rates
- Swap between selected currencies
- Responsive and clean UI

## Technologies Used
- React.js
- Tailwind CSS (for styling)
- JavaScript (ES6+)
- Fetch API (for fetching currency exchange data)

## Project Structure
```
📂 currency-converter-app
├── 📂 src
│   ├── 📂 components
│   │   ├── InputBox.js      # Custom input component for currency selection
│   │   ├── index.js        # Exports components
│   ├── 📂 hooks
│   │   ├── useCurrencyInfo.js  # Custom hook to fetch currency data
│   ├── App.js              # Main application logic
│   ├── index.js            # Entry point of the app
├── 📄 README.md            # Project documentation
├── 📄 package.json         # Dependencies and project configuration
```

## Installation

### Prerequisites
Make sure you have **Node.js** and **npm** installed.

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/currency-converter-app.git
   ```
2. Navigate to the project folder:
   ```bash
   cd currency-converter-app
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Start the development server:
   ```bash
   npm start
   ```
5. Open the browser and go to:
   ```
   http://localhost:3000
   ```

## Usage
1. Enter an amount in the **From** currency input box.
2. Select the currency type from the dropdown.
3. Choose the currency to **convert to** from the dropdown.
4. Click on the **Convert** button.
5. The converted amount will be displayed in the **To** currency input box.
6. Click the **Swap** button to reverse the currency conversion.

## API Integration
The app fetches real-time exchange rates from:
```
https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@{date}/v1/currencies/{currency}.json
```
Example for USD:
```
https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@2025-02-15/v1/currencies/usd.json
```

## Components Breakdown
### 1. `App.js`
- Manages state for currency conversion.
- Fetches currency rates using `useCurrencyInfo` hook.
- Renders `InputBox` components for user interaction.
- Handles **swap** and **convert** logic.

### 2. `useCurrencyInfo.js` (Custom Hook)
- Fetches exchange rates for a selected currency.
- Updates data dynamically when the selected currency changes.

### 3. `InputBox.js`
- Custom input component for entering amounts and selecting currency types.
- Uses the `useId()` hook for accessibility.

## Future Enhancements
- Add **historical exchange rates**.
- Implement a **dark mode**.
- Improve UI with **better animations**.
- Add more **currency conversion options**.

## Contributing
Feel free to fork this repository and submit pull requests! 😊

## License
This project is licensed under the **MIT License**.

