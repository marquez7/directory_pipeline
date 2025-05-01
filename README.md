# Directory_Dipeline
##########################################################
# CREATING A DATA PILINE OUT OF A FOLDER IN A DIRECTORY  #
##########################################################

A. Purpose: 
      1.The purpose of this document is to develope a data pipiline out of a folder using python only. Currently, there are automated tools that can make developing data pipelines 
    	easier, however, due to network security in most jobs/ work places the ability to download these programs is often limited, or isn't possible especially if you have a locked network, 
      thus we have to work with what we have.
      II. Mapping of Methodology
B Thought Process
	1.  Each metric will have a folder to serve as a repository to hold exported reports from HMIS.
		a. ClientsInPrograms Data Pull will feed the following reports:
			*Demographics
			*Positive Exits for Housing/Outreach Programs
			*New Clients Housed
			*Current Clients Housed
		b. CoC Caper Report Data Pull will feed the following reports:
			*Increased in Earned Cash
			*Increase in Non-Cash
3. Workflow process .
	a. For each folder-->
		- We need to take each file in the folder-->
			-clean the data as needed-->
				-then add the necessary columns for computing / data tracking
				*column for the source of the data- to ensure we know the file location of the datapoint
				*column for with the date the file was processed (To identify the time frame the data belongs too/ and also identify the date the error was processed)
	b. Next we need to then load the data into a parquet file for aggregation
	purposes.
		- The parquet file is used to maintain the integrity of the data types for
		further analysis, and to be 
  		- Will also be used for the PowerBI dashboard/ Tableau
	c. Next we need to archive the processed parquet file data to a .csv file so the data can be readable after processed by those who need to review the data.
		- Parquet files are binary files are serialized and are not human readable.
		-having a .csv file will allow others to read the data should they need too.



