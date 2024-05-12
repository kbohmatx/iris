# Create a class 
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
