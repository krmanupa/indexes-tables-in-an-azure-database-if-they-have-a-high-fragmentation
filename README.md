Indexes tables in an Azure database if they have a high fragmentation
=====================================================================

            

This runbook indexes all of the tables in a given database if the fragmentation is above a certain percentage. It highlights how to break up calls into smaller chunks, in this case each table in a database, and use checkpoints.


This allows the runbook job to resume for the next chunk of work even if the fairshare feature of Azure Automation puts the job back into the queue every 30 minutes.


You could schedule this runbook to run every night to ensure that your database indexes remain optimized.


 

 

        
    
Note: TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group.
