# RPA Project - Formula 1 Driver Statistics

## Team Members:
- **Apostol Alin-Constantin** (alin-constantin.apostol@s.unibuc.ro) - Group 351
- **Colțoș Radu-Mihai** (radu-mihai.coltos@s.unibuc.ro) - Group 351
- **Grigore Mihai** (mihai.grigore1@s.unibuc.ro) - Group 352
- **Pîrvulescu Daria-Maria** (daria-maria.pirvulescu@s.unibuc.ro) - Group 351

## Project Idea

### Input:
A file containing information about one or more Formula 1 drivers.

### Output:
An email containing one or more Excel files with statistics about the drivers extracted from the input file.

### Description:
The robot is manually activated with an input file that contains specific information about the drivers we want to process. This information can include the driver's name, nationality, team, etc.

The robot searches for information about all the drivers in the championship on the [f1.com](https://www.f1.com) website using **Table Extraction (data scraping)**. It then performs certain analyses and saves the results in an Excel file, which is finally sent via email.

During the information search on the internet, the robot will also record the browser's initiated requests using a **Web Request Trigger** (a new addition as of 24.10, this feature is not yet documented as it was recently introduced upstream and implemented by one of the team members 😊).

### Technologies Used:
- **Modern Activities**: These are necessary for the Web Request Trigger. Additionally, modern activities are more reliable than classic activities and do not require extra checks like "Element Exists." This is because activities interacting with UI elements (i.e., those in the UI Automation package) are dependent on the parent application context (Use Application/Browser).

---

This project aims to automate the process of gathering and analyzing Formula 1 driver statistics, making it easier to generate and share insights via email.
