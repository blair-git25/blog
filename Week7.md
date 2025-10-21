# Week 7
___
## Learning Outcome 3

**_1. Write a paragraph describing the function and importance of making regular backups and give an example of an appropriate backup strategy. You should also mention the choice of media used, and why; and the importance of regularly testing the backup media._**

**_Discuss some common methods for the recovery of deleted data. Include a description of at least one commercially available utility useful for this purpose._**

#### 1. Regular backups


A regular backup is done by creating copies of data (can be critical or non-critical) and storing them separately from the original (usually on another disk). This can be done a time intervals of hours/days/weeks etc. 

It is important to make regular backups for redundancy. Backups allow data to be restored if it’s been accidentally deleted, corrupted/damaged, system bugs/crashes or through theft/ransomware. Also data must be kept to comply with certain legal requirements. 

##### Backup Strategy

An appropriate backup strategy would be to use tapes for daily/weekly and yearly backups. Tapes are recommended as they offer high capacity and longevity, which makes them ideal for long-term archiving and off-site storage.  

Hourly disk snapshots (e.g. through NetApp) can be used for rapid data recovery, but will not be held long term. These are quicker to recover/access data compared to tapes. 

##### Verify backups

It's important to regularly test backup media to ensure and verify your backups are actually usable when you need them. Untested backups are essentially just hope, not a reliable recovery plan. 

Testing confirms the backed up data can be readable and recovered when needed. Media can degrade over time and data can be corrupted during the backup process, checking can ensure the availability of data when you need it. Documenting testing of backups can add to compliance for security policies. 

#### 2. Commercial data recovery

Common methods of deleted data recovery can range from simply recovering items from your Recycle Bin or via disk cloning and the use of software to access the raw data to find data file signatures

A commonly used commercial data recovery tool is DiskDigger. DiskDigger is a data recovery program that can recover lost files from storage media like hard drives, memory cards and USB drives. 
DiskDigger works by scanning the raw disk sectors for known file signatures. This process allows it to find and reconstruct deleted data (photos, documents and videos) even from drives that have been reformatted.