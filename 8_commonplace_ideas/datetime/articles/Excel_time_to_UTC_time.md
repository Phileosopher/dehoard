# The problem

I had a CSV file that needed to be processed on a web page. So I had to convert the Excel time to UTC time.

# The solution

According to [this answer on StackOverflow](https://stackoverflow.com/a/32848723/319711):
> The Excel number for a modern date is most easily calculated as the number of **days** since 12/30/1899 on the Gregorian calendar.
>
> Excel treats the mythical date 01/00/1900 (i.e., 12/31/1899) as corresponding to 0, and incorrectly treats year 1900 as a leap year. So for dates before 03/01/1900, the Excel number is effectively the number of days after 12/31/1899.

UTC time is represented in JavaScript as the number of **milliseconds** since 1/1/1970, so there are effectively:
- 70 years between the two starting points
- Plus 1 day as Excel starts at 31 Dec
- Plus 17 leap years in that period
- Plus 1 day as Excel treats 1900 incorrectly as a leap year too (this only applies for dates after 1 March 1900).

This means that the Excel time is 70 * 365 + 1 + 17 + 1 = 25569 days before the UTC start. 
As one day is 24 * 60 * 60 = 86400 seconds or 86400 * 1000 milliseconds, you get:

> utcTime = (excelTime - 25569) * 86400000

## Note
- Since Excel writes large numbers with an exponent, you may prefer to save the number in seconds, 
and multiply by 1000 in JavaScript (it will make the file much smaller too)
- Beware that you may have to compenstate for the timezone offset. E.g. in the Netherlands, 
the reported time is likely given using GMT+1, so you need to additionally subtract one hour too, 
giving you the following formula:

> utcTime = ((excelTime - 25569) * 86400 - 3600) * 1000
