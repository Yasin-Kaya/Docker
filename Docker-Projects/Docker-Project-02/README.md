# Project-02 : Roman Numerals Converter Application (Python Flask) deployed on AWS EC2 with Terraform

## Description
Roman Numerals Converter App aims to convert given number to Roman numerals. The application will be coded in Python and deployed as a web application with Flask on AWS Elastic Compute Cloud (EC2) Instance using Terraform. The application will be run on EC2 using Docker image.

## Problem Statement

![Project_001](Docker-Project-02-1288.jpg)

- Your company has recently started on a project that aims to be one of the most used unit converters and formulas website. Roman Numerals Converter is the part of the project. So you and your colleagues have started to work on the project.

- As a first step of the project, developers wrote a basic Python Flask program that converts the given number (between 1 and 3999) to the roman numerals. The program converts only from numbers to Roman numerals, not vice versa and during the conversion following notes should be taken into consideration.
   
```
Roman numerals are represented by seven different symbols: I, V, X, L, C, D and M.
- Symbol       Value
- I             1
- V             5
- X             10
- L             50
- C             100
- D             500
- M             1000
- For example, two is written as II in Roman numeral, just two one's added together. 
Twelve is written as, XII, which is simply X + II. 
The number twenty seven is written as XXVII, which is XX + V + II.
- Roman numerals are usually written largest to smallest from left to right. 
However, the numeral for four is not IIII. Instead, the number four is written as IV. 
Because the one is before the five we subtract it making four. 
The same principle applies to the number nine, which is written as IX. 
There are six instances where subtraction is used:
- I can be placed before V (5) and X (10) to make 4 and 9. 
- X can be placed before L (50) and C (100) to make 40 and 90. 
- C can be placed before D (500) and M (1000) to make 400 and 900.
```

- User input can be either integer or string, thus the input is checked for the followings,

   - The input should a decimal number within the range of 1 to 3999, inclusively.
   
   - If the input is less then 1 or greater then 3999, program warns the user using the given html template.

   - If the input is string and can not be converted to decimal number, program warns the user using the given html template.

- Example for user inputs and respective outputs

```
Input       Output
-----       ------
3           III
9           IX
58          LVIII
1994        MCMXCIV
-8          Warning with "Not Valid! Please enter a number between 1 and 3999, inclusively."
4500        Warning with "Not Valid! Please enter a number between 1 and 3999, inclusively."
Ten         Warning with "Not Valid! Please enter a number between 1 and 3999, inclusively."
```
   
- As a DevOps, developer has given you app and template folder, you are requested to deploy your web environment using Python's Flask framework.

- You are requested to push your program to the project repository on the Github and deploy your solution in the development environment on AWS EC2 Instance using Terraform to showcase your project. In the development environment, you'll configure your Terraform template using the followings,

   - The application stack should be created with new AWS resources. 

   - Should take the name of your Key Pair and write it in The terraform tf file ;
   
   - The application should run on Amazon Linux 2 EC2 Instance

   - EC2 Instance type can be configured as `t2.micro`.

   - Latest AWS Linux AMI should be used for template.

   - Instance launched by Terraform should be tagged `Docker` 

   - The Web Application should be accessible via web browser and terminal from anywhere.

   - The Application files should be downloaded from Github repo and deployed on EC2 Instance using user data script within Terraform. 

   - Roman Numerals Converter Application Website URL should be given as output by Terraform, after the tf file is created.

- Lastly, try to deploy same infrastructure using AWS CLI commands to showcase your project. 

## Project Skeleton 

```
001-roman-numerals-converter (folder)
|----cli.sh            # Requested (CLI commands)
|----readme.md         # Given (Definition of the project)          
|----cfn-template.yml  # Requested (Cloudformation template)
|----app.py            # Given (Definition of the project)          
|----templates
        |----index.html  # Given (HTML template)
        |----result.html # Given (HTML template)
```

## Expected Outcome

![Project 001 Snapshot](Romen-Number-01.jpg)

### At the end of the project, following topics are to be covered;

- Algorithm design

- Programming with Python 

- Web application programming with Python Flask Framework 

- Bash scripting

- AWS EC2 Service

- AWS Security Groups Configuration

- Terraform Tf File

- AWS CLI Service

- AWS CLI commands, filters and queries

- Git & Github for Version Control System

### At the end of the project, your will be able to;

- improve coding skills using iterables(dict), operators, for-loop, if statements and functions within Python

- improve web programming skills using HTTP GET/POST methods, template formatting, importing packages within Python Flask Framework

- improve bash scripting skills using `user data` section in Terraform to install and setup web application on EC2 Instance

- configure AWS EC2 Instance and Security Groups.

- configure Terraform tf file to use AWS Resources.

- use AWS Cli to launch same tf file.

- use git commands (push, pull, commit, add etc.) and Github as Version Control System.

## Steps to Solution
  
- Step 1: Download or clone project definition from `Kaya-Y` repo on Github 

- Step 2: Create project folder for local public repo on your pc

- Step 3: Copy the Roman Numerals Converter Application in Python

- Step 4: Prepare a terraform tf file to deploy your app on EC2 Instance

- Step 5: Push your application into your own public repo on Github

- Step 6: Deploy your application on AWS Cloud using terraform tf file to showcase your app within your team.

- Step 7: Deploy your application on AWS Cloud using AWS Cli to showcase your app within your team.

## Notes

- Customize the application by hard-coding your name for the `developer_name` variable within html templates.

## Resources

- [Python Flask Framework](https://flask.palletsprojects.com/en/1.1.x/quickstart/)

- [Python Flask Example](https://realpython.com/flask-by-example-part-1-project-setup/)

- [Terraform AWS Provider](https://registry.terraform.io/providers/hashicorp/aws/latest/docs)

- [AWS Cli User Guide](https://docs.aws.amazon.com/cli/latest/)

## Contact

- Please contact me to access the project files.
    * yasinkaya.devops@gmail.com