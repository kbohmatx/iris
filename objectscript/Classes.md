# Create a class 
https://learning.intersystems.com/course/view.php?name=IRIS%20Class

Class Demo.Company Extends (%Persistent, %Library.Populate)
{
/// Name
Property Name As %String [ Required ];
Property YearsActive As %Integer;
Property Industry As %String;
...


# Instantiate a class
set company = ##class(Demo.Company).%New()

# Set a property on the class
set company.Name = "InterSystems"

set company.YearsActive = 40

set company.Industry = “Technology”

do company.PrintCompany()
