# Directory_Dipeline
##########################################################
# CREATING A DATA PILINE OUT OF A FOLDER IN A DIRECTORY  #
##########################################################

	A. Purpose: 
      1.The purpose of this document is to develope a data pipiline out of a folder using python only. Currently, there are automated tools that can make developing data pipelines 
    	easier, however, due to network security in most jobs/ work places the ability to download these programs is often limited, or isn't possible especially if you have a locked network, 
      thus we have to work with what we have.


--------[RAW Exports from - HIPPA Regulated DB]------
            ______/¯¯¯|                                     |
            |Metric2  |>------\-------->\                   |
            |_________|        |         \                  |
                               |          \                 |
             ______/¯¯¯|       |            _______/¯¯¯¯|   | 
            | Metric1  |>------|---------> | Parquet    |   |------------> [Dash Board]
            |__________|       |          |_____________/   |  
                               |                            |
             ______/¯¯¯|       |         /                  |
            | Metric3  |>------|------->/                   |
            |__________|       |                            |
                               |                            |
            ______/¯¯¯|        |                            |
            | Archive | <------|                            |
            | M1,M2,M3|                                     |
            |_________|                                     |
    |________________________________________________________

            
