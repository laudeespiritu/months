# months #
Different formatting of Months in JSON. Useful for those who just want to get all the months without using libraries.

Available Formats:
- Simple (Complete name and First three letters)
- Comprehensive:

Class         | Value
------------- | -------------
name          | Complete name
short         | Shortened name
number        | Number of month
days          | Total days although February can vary because of leap year

## Sample Usage (JavaScript) ##
```
let monthsJson = JSON.parse('<%path/to/file%>/months.json');

/////////////////////////////
// Simple
/////////////////////////////
let monthsSimple    = monthsJson.monthsSimple;
let monthsComplete  = monthsSimple.complete; // E.g. "January"
let monthsShort     = monthsSimple.short; // E.g. "Jan"

/////////////////////////////
// Comprehensive
/////////////////////////////
let monthsComplete = monthsJson.monthsComprehensive;
monthsComplete[0].name    // E.g. "January"
monthsComplete[0].short   // E.g. "Jan"
monthsComplete[0].number  // E.g. 1
monthsComplete[0].days    // E.g. 31
```

## Credits ##
Thanks to [@brandonwamboldt](https://github.com/brandonwamboldt) for the detailed reference for the months.
