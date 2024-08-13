## Currency Converter 

This is a readme file for a currency converter webpage built with JavaScript.

### Features

* Convert between various currencies using real-time exchange rates.
* User-friendly interface with dropdown menus for selecting currencies.
* Country flags displayed for each selected currency.
* Handles empty or invalid input for conversion amount (defaults to 1).

### Screenshots of the Interface



### Technologies Used

* HTML
* CSS 
* JavaScript (ES6)
* External libraries:
    * [@fawazahmed0/currency-api](https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@latest/v1/currencies/) - Fetches real-time exchange rates.
    * [Flags API](https://www.flagsapi.com/) - Provides country flag images.

### Getting Started

1. **Clone the repository or download the source code.**
2. **Open the index.html file in a web browser.**
3. **Select the currencies you want to convert between from the dropdowns.**
4. **Enter the amount you want to convert (default is 1).**
5. **Click the "Convert" button to see the converted amount.**

### Code Breakdown

* The `countryList` object maps currency codes to country codes.
* The `BASE_URL` variable defines the base URL for the currency API.
* The code selects necessary DOM elements using `querySelectorAll` and `querySelector`.
* Default currency values (`fromCountry` and `toCountry`) are initialized.
* A loop iterates through `countryList` to populate the dropdown menus with options for each currency code.
* The `updateFlag` function updates the country flag image based on the selected currency code.
* The `updateExchangeRate` function fetches exchange rates from the API and displays the converted amount.

### Dependencies

This code relies on the following external links:

* @fawazahmed0/currency-api [(https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@latest/v1/currencies/)](https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@latest/v1/currencies/)
* Flags API ([https://www.flagsapi.com/](https://www.flagsapi.com/))

### Additional Notes

* This code provides a basic implementation of a currency converter. You can further customize it by adding features like historical exchange rates, charting functionality, or support for more currencies.
