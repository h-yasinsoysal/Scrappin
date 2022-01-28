# Scrappin - Updated 2021
  
Scrappin is a profile scraping tool for LinkedIn. Given a company name, it goes through a predefined list of departments and returns the employees, their job title, their work experience, and many more.

## First Steps

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

Write the command:

```
git clone https://github.com/huarstudios/Scrappin.git
```

Within the directory, run the command:

```
python scrappin.py -h
```
Your output will be
```
usage: scrappin.py [-h] [--company string] [--emps file]
                           [--emailformat string]

Scrappin - Profile Scraper build H.Y. Soysal

optional arguments:
  -h, --help            show this help message and exit

Company Name:
  --company string      Enter the company name  
  
Employee Digging:
  --emps file           Discover employees by title and/or department. Titles
                        and departments are imported from a new line delimited
                        file. [Default: title-list-small.txt]
  --emailformat string  Create email addresses for discovered employees using
                        e-mail format. [Accepted Formats: first.last@sample.com,
                        last.first@sample.com, firstl@sample.com, lfirst@sample.com,\
                        flast@sample.com, lastf@sample.com, first@sample.com,
                        last@sample.com]
```

As a demonstration of the program's ability, enter:

```
python scrappin.py --company "sample company name" --emps "/home/lider/scraper/wordlists/title-list-small.txt" --email: first.last@samplecompany.com
```
The output 

```
---------------------------------------------------------------
FINANCE
---------------------------------------------------------------

NAME: Jonnahtan Doe
---------------------
Education:
-  ABC College
Experience:
-  Director, Financial Planning &amp; Analysis at Sample Company
-  Manager - Finance at AWS
Job Title:
-  Director, Financial Planning &amp; Analysis at Sample Company
EMAIL: jonatthan.doe@samplecompany.com 

NAME:Jonnathan Doe
---------------------
Education:
-  Sample University
-  Sample High School
Experience:
-  Finance Intern at Sample Company 
Job Title:
-  Intern at Sample Company
EMAIL: johatthan.doe@samplecompany.com

