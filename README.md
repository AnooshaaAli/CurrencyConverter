## Currency Converter 

This is a readme file for a currency converter webpage built with JavaScript.

### Features

* Convert between various currencies using real-time exchange rates.
* User-friendly interface with dropdown menus for selecting currencies.
* Country flags displayed for each selected currency.
* Handles empty or invalid input for conversion amount (defaults to 1).

### Screenshots of the Interface

##Default View

![image](https://github.com/user-attachments/assets/f2ef7efb-32a3-49a3-aee7-cff2bc761f1a)

##100USD TO PKR

![image](https://github.com/user-attachments/assets/0f573057-a524-4315-bacb-27691f0225f0)

##10EUR TO PKR

![image](https://github.com/user-attachments/assets/2571e5c8-8ecb-44fa-aa98-11e035b1c84f)

##10AUD TO JPY

![image](https://github.com/user-attachments/assets/e8784553-87eb-4b7d-a27f-ac5212e919fd)

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
