# Tastamat Widget

This widget should be used to 

## Steps to integrate Tastamat Widget

1. Include CSS style:

    Copy this line of code and paste it into the `<head/>` part of the page:
    ```
    <link href="https://tastamat.kz/widget/style.css" rel="stylesheet">
    ```

2. Place the widget:

    Place the following `<div/>` element to the specified part of the page:
    ```
    <div id="tastamatWidget" class="tstmtWdgt__main"></div>
    ```

3. Add script:

    Add the following script to the end of the `<body/>` element and specify necessary attributes:

    ```
    <script
        type="text/javascript"
        src="https://tastamat.kz/widget/script.js"
        data-width="500px"
        data-height="500px"
        data-apikey="<YANDEX_MAPS_API_KEY>"
        data-addressid="<idOfTheAddressInputElement>"
        data-cityid="<idOfTheCityInputElement>"
        data-indexid="<idOfTheZipCodeInputElement>"
    ></script>
    ```

    Mandatory attributes:

    - data-width - width of the widget
    - data-height - height og the widget
    - data-apikey - Yandex API key (can be issued on the Yandex for Developer portal at https://tech.yandex.com/) - _Go to the [Developer's Dashboard](https://developer.tech.yandex.ru) page and click Get key. In the popup window, select the “JavaScript API and Geocoder HTTP API”. After you select the service, a form appears. In this form, you need to provide your contact information. After you fill in the form, the “Service successfully connected” text appears. The created key is now available in the “Keys” section. Use it when you enable the API._
    
    Additional attributes:

    - data-addressid - `<input>` HTML element ID for address
    - data-cityid - `<input>` HTML element ID for city name
    - data-indexid - `<input>` HTML element ID for zip code (postal code)

    _(these fields will be automatically filled when "Выбрать" button pressed)_
