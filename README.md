# CRM-SYSTEM
Customer  relationship management system becomes online. 

/*The code for CRM application in JavaScript is below/

form Add_Leads
{
	displayname = "Add Leads"
	success message = "Data Added Successfully!"
	field alignment = left
	Section
	(
		type = section
	 	row = 1
	 	column = 0   
		width = medium
	)
	Lead_Status
	(
		type = picklist
		displayname = "Lead Status"
		values = {"New", "Nurturing", "Choice"}
	 	row = 1
	 	column = 1   
		width = medium
	)
	Name
	(
    	type = name
     	prefix
     	(
	     	 type = prefix
	     	 displayname ="Prefix"
	     	 visibility = false
	     	 value = {"Mr.","Mrs.","Ms."}
     	) 
     	first_name
     	(
	     	 type = first_name
	     	 displayname ="First Name"
     	) 
     	last_name
     	(
	     	 type = last_name
	     	 displayname ="Last Name"
     	) 
     	suffix
     	(
	     	 type = suffix
	     	 displayname ="Suffix"
	     	 visibility = false
     	) 
	 	row = 1
	 	column = 1   
		width = medium
	)
	must have Phone_Number1
	(
    	type = phonenumber
		displayname = "Phone Number"
    	allowedcountries={in}
    	defaultcountry="in"
	 	row = 1
	 	column = 1   
		width = medium
	)
	Address
	(
    	type = address
     	capture_coordinates = true
     	adjust_using_map = false
     	address_line_1
     	(
	     	  type = address_line_1
	     	  displayname = "Address Line 1"
     	) 
     	address_line_2
     	(
	     	  type = address_line_2
	     	  displayname = "Address Line 2"
     	) 
     	district_city
     	(
	     	  type = district_city
	     	  displayname = "City / District"
     	) 
     	state_province
     	(
	     	  type = state_province
	     	  displayname = "State / Province"
     	) 
     	postal_Code
     	(
	     	  type = postal_Code
	     	  displayname = "Postal Code"
     	) 
     	country
     	(
	     	  type = country
	     	  displayname = "Country"
     	) 
     	latitude
     	(
	     	  type = latitude
	     	  displayname = "latitude"
	     	 visibility = false
     	) 
     	longitude
     	(
	     	  type = longitude
	     	  displayname = "longitude"
	     	 visibility = false
     	) 
	 	row = 1
	 	column = 1   
		width = medium
	)
	Business_Name
	(
    	type = text
		displayname = "Business Name"
	 	row = 1
	 	column = 1   
		width = medium
	)
	Official_Number
	(
    	type = phonenumber
		displayname = "Official Number"
	 	row = 1
	 	column = 1   
		width = medium
	)
	must have Email
	(
    	type = email
	 	row = 1
	 	column = 1   
		width = medium
	)
	must have Website
	(
    	type = url
		enable  linkname
	 	row = 1
	 	column = 1   
		width = medium
	)
	Office_Address
	(
    	type = address
		displayname = "Office Address"
     	capture_coordinates = true
     	adjust_using_map = false
     	address_line_11
     	(
	     	  type = address_line_1
	     	  displayname = "Address Line 1"
     	) 
     	address_line_21
     	(
	     	  type = address_line_2
	     	  displayname = "Address Line 2"
     	) 
     	district_city1
     	(
	     	  type = district_city
	     	  displayname = "City / District"
     	) 
     	state_province1
     	(
	     	  type = state_province
	     	  displayname = "State / Province"
     	) 
     	postal_Code1
     	(
	     	  type = postal_Code
	     	  displayname = "Postal Code"
     	) 
     	country1
     	(
	     	  type = country
	     	  displayname = "Country"
     	) 
     	latitude1
     	(
	     	  type = latitude
	     	  displayname = "latitude"
	     	 visibility = false
     	) 
     	longitude1
     	(
	     	  type = longitude
	     	  displayname = "longitude"
	     	 visibility = false
     	) 
	 	row = 1
	 	column = 1   
		width = medium
	)
	Product
	(
    	type = text
		displayname = "Product ID"
	 	row = 1
	 	column = 1   
		width = medium
	)
	Lead_Type
	(
		type = picklist
		displayname = "Lead Type"
		values = {"Hot", "Cold", "Warm"}
	 	row = 1
	 	column = 1   
		width = medium
	)
	
	actions
	{
		on add
		{
			submit
			(
   				type = submit
   				displayname = "Submit"
			)
			reset
			(
   				type = reset
   				displayname = "Reset"
			)
		}
		on edit
		{
			update
			(
   				type = submit
   				displayname = "Update"
			)
			cancel
			(
   				type = cancel
   				displayname = "Cancel"
			)
		}
	}
}
