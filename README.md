# Python JSON to CSV
To convert JSON to CSV in Python, use the pandas to_csv() function. The to_csv() is a Pandas library function you can use in Python that writes objects to a comma-separated values (csv) file. To convert Python JSON to CSV, we first need to read json data using the Pandas read_json() function and then convert it to csv.

To use json in Python, we have to import the json package in Python script. The JSON text is done through quoted-string, which contains the value in key-value mapping within { }. It is similar to the Dictionary in Python

CSV (Comma Separated Values) is the simple file format used to store tabular data, such as databases or spreadsheets.



# Steps to Convert a Python JSON to CSV
Follow the below steps one by one to convert JSON to CSV in Python.

1. Get the JSON Data.
2. Read the data and transform it into a Pandas object.
3. Convert Pandas object to CSV
4. Downloading the csv file



# Step 1: Get JSON Data

The contents of the file are following. 

```json
{
  "0": {
    "Netflix": "Stranger Things",
    "Quibi": "Most Dangerous Game"
  },
  "1": {
    "Netflix": "Money Heist",
    "Quibi": "The Stranger"
  },
  "2": {
    "Netflix": "House of Cards",
    "Quibi": "50 States of Fright"
  },
  "3": {
    "Netflix": "Rick and Morty",
    "Quibi": "Flipped"
  },
  "4": {
    "Netflix": "Better Call Saul",
    "Quibi": "Survival"
  }
}

```

In the above file, you can see that the keys are index. That means, when we convert it into a pandas object, the index would be 0, 1, 2, 3, 4, and header columns will be Netflix and Quibi.



# Step 2: Read json and transform it into Pandas object
Pandas read_json() is an inbuilt function that converts a JSON string to a pandas object. Parsing of the JSON Dataset using pandas is much more convenient. Pandas allow you to convert the list of lists to DataFrame and specify the column names separately.

A JSON parser transforms a JSON text into another representation must accept all texts that conform to the JSON grammar.

I am assuming that the export.json file is in the same directory as your coding file. So your path is just a filename. Let’s transform the JSON string to Pandas object.



# Step 3: Convert Pandas Object to CSV
Let’s convert Pandas object to CSV data and print it in the console.



# Step 4: Donwloading the csv file
Here, we have downloaded the CSV data. We can also print CSV data here. To do that, we need to provide the export path to create a CSV file. Let’s say we are exporting in the same directory as the export.json file.

In this case, we don’t need to return any data because we are exporting the file. So that is why the returning value here is None.

The exported file’s name is the streaming.csv file, in the same directory as the export.json file.