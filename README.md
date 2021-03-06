# Quick Date Input

This widget allows users to quickly enter dates.
 
## Description

The user can enter the date in any of the following formats:

### DDMM
The year will be determined based on the setting of the "Current Year" boolean. By default the "Current Year" is set to true and the missing year information will be interpreted as the current year. When the "Current Year" is set to false the date will be interpreted as the current or next possible date.

### DDMMYY
The date is considered to be in the current century.

### DDMMYYYY
There is no information missing.

## Example use
*All dates are in the DD/MM/YYYY format.*

|System Date|Input|CurrentYear|Output|
|---|---|---|---|
|27/03/2016|2603|true|26/03/2016|
|27/03/2016|2603|false|26/03/2017|
|27/03/2016|260321|not applicable|26/03/2021|
|27/03/2016|26032021|not applicable|26/03/2021|

## Validations
Any seperators used in the input are ignored. The output date uses /'s as seperator.
Validation errors are shown when the input contains letters or when the input can not result in a valid date (e.g. 29/02/2001).