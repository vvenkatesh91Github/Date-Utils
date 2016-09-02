Creates the DateUtils object.
var date = new DateUtils();

Sample Date Formats
	date.getFormats();
	{
			"year" : ["10", "2016"],
			"month" : ["08", "Aug", "August"],
			"day" : ["01", "1st", "Mon", "Monday"],
			"hours" : ["01", "13"],
			"minutes" : ["59"],
			"seconds" : ["59"],
			"milliSeconds" : ["999"],
			"meridiem" : ["pm"]
	};

	date.getDate();
Returns the set date as string in the form of dd/mm/YYYY.

Formats the date as required.
	Prototype - formatDate(outformat, date, informat);
	
	date.formatDate("dd/mm/YYYY") - Formats current date
	date.formatDate("dd/mm/YYYY", "Aug-01-2015", "MMM-dd-YYYY") - formats input date.
	
Get days of a month
	date.daysOfMonth(month, year);
	
	month may be in any format - "08" or "Aug" or "August".
	year may be in any formats - "16" or "2016"
	
To find year is leap year or not
	date.isLeapYear(year);
	
	year may be in any formats - "16" or "2016"
	
To add Hours
	Prototype - addHour(nHours, date, format)
	
	Example:
	date.addHour(nHours) - Adds hours to the current date.
	date.addHour(nHours, "Aug-01-2015 09:40", "MMM-dd-YYYY hh:ii") - Adds hours to the input date. Date and month should be mandatory.
		
To Subract Hours
	Prototype - subHour(nHours, date, format)
	
	Example:
	date.subHour(nHours) - Subracts hours to the current date.
	date.subHour(nHours, "Aug-01-2015 09:40", "MMM-dd-YYYY hh:ii") - Subracts hours to the input date. Date and month should be mandatory.
	
To Add days
	Prototype - addDay(nDays, date, format)
	
	Example:
	date.addDay(nDays) - Adds days to the current date.
	date.addDay(nDays, "Aug-01-2015 09:40", "MMM-dd-YYYY hh:ii") - Adds days to the input date.
	
To Subract days
	Prototype - subDay(nDays, date, format)
	
	Example:
	date.subDay(nDays) - Subracts days to the current date.
	date.subDay(nDays, "Aug-01-2015 09:40", "MMM-dd-YYYY hh:ii") - Subracts days to the input date.
	
To Add Months
	Prototype - addMonth(months, date, format)
	
	Example:
	date.addMonth(months) - Adds months to the current date.
	date.addMonth(months, "Aug-01-2015 09:40", "MMM-dd-YYYY hh:ii") - Adds months to the input date.
	
To Subract Months
	Prototype - subMonth(months, date, format)
	
	Example:
	date.subMonth(months) - Subracts days to the current date.
	date.subMonth(months, "Aug-01-2015 09:40", "MMM-dd-YYYY hh:ii") - Subracts months to the input date.
	
To Add year
	Prototype - addYear(years, date, format)
	
	Example:
	date.addYear(years) - Adds year to the current date.
	date.addYear(years, "Aug-01-2015 09:40", "MMM-dd-YYYY hh:ii") - Adds year to the input date.
	
To Subracts year
	Prototype - subYear(years, date, format)
	
	Example:
	date.subYear(years) - Subracts year to the current date.
	date.subYear(years, "Aug-01-2015 09:40", "MMM-dd-YYYY hh:ii") - Subracts year to the input date.
	
To Compare Date
	prototype - compareDate(date1, format1, date2, format2);

	Example:
	date.compareDate("26-08-2016 10:29:54:544 AM", "dd-mm-YYYY hh:ii:ss:mi ap", "Aug 26 16 10-29 54:543 AM", "MMM dd yy hh-ii ss:mi ap")
