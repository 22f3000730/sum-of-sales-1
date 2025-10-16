# Sales Summary Application

This single-page web application fetches sales data from an encoded CSV file, calculates the total sales, and displays the result.

## Features

- Fetches and processes CSV data from a base64 encoded data URI
- Calculates the sum of the sales column
- Displays the total sales in a Bootstrap-styled interface
- Uses Bootstrap 5 from jsDelivr CDN
- Sets the document title as specified

## Implementation Details

1. The application fetches data from: `data:text/csv;base64,aXRlbSxzYWxlcwpBcHBsZXMsMTIwLjUwCkJhbmFuYXMsODUuNzUKT3JhbmdlcywxNTAuMjUKR3JhcGVzLDk5LjAwCk1hbmdvZXMsMTMwLjQwCg==`
2. Parses the CSV content to extract sales values
3. Calculates the sum of all sales values
4. Displays the total in the element with id `total-sales`
5. Uses the exact title specified in the requirements
6. Loads Bootstrap 5 from jsDelivr CDN

## Error Handling

The application includes basic error handling for:
- Network issues while fetching the CSV data
- Data parsing problems
- Invalid sales values

In case of errors, the application will display "Error" in the total sales field and log the error to the console.

## Compliance

This implementation complies with all specified requirements:
- Uses the exact title specified
- Loads Bootstrap from jsDelivr
- Displays the calculated total in the element with id `total-sales`
- Processes the base64 encoded data URI correctly
- Maintains the template literal syntax in the data URI