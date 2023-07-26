**Google Maps Data Retrieval Script**

This script is designed to retrieve useful information such as addresses, geolocation (latitude and longitude), phone numbers, emails, and opening hours for a list of target customers using the Google Maps API. To use this script, you will need a valid Google Maps API key.

**Prerequisites**

Before running the script, you need to install the googlemaps library.
You can do this via pip:

+ pip install -U googlemaps

**Getting started**

+ Sign up for a Google Cloud account and enable the Google Maps API.
+ Create an API key by following the instructions in the Google Cloud Console.
+ Replace 'API_ADDRESS' in the script with your actual API key.

**Usage**

The script uses the Google Maps API to retrieve data for a list of target customers. Make sure you have a list of target customer names (stored in target_customers_list) for which you want to retrieve data.
Replace target_customers_list with your list of target customers' names.
Run the script.

**Script Description**

+ The script uses the Google Maps API to initialize a client, which allows you to make requests to the API using your API key.
+ Empty lists are created to store the data for each target customer, including addresses, latitude, longitude, phone numbers, emails, and opening hours.
+ The script loops through the target_customers_list and tries to retrieve data for each customer using the Google Maps API.
+ If the data is successfully retrieved, the script extracts the relevant information from the API response and appends it to the respective lists.
+ If there is an issue with retrieving data for a specific customer (e.g., no information found, API error), the script sets the corresponding values to None in the lists.
+ After the script finishes running, the lists will contain the relevant data for each target customer, which you can use for further analysis or storage.

Please note that the script is designed to handle exceptions gracefully, so if any issues occur during the data retrieval process, it will not terminate abruptly and will continue processing the remaining customers.

**Important Note**

Be mindful of Google Maps API usage limits and billing. Depending on the number of requests made, you may incur charges or encounter rate-limiting issues. Refer to the Google Maps API documentation and billing information for more details.

Always ensure compliance with Google's Terms of Service and usage policies when using the API.
