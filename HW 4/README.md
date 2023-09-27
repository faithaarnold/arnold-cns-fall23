# 1/c Faith Arnold - CNS Homework #4 - 27 September 2023 
## Creating AD Users
Using the Active Directory Users and Computers GUI, we were each able to create a new user under the ad.snickerdoodle.com domain. The users we created only have user privileges. Below is a screenshot of the user I created to use on the domain.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/7cb8a98e-ea41-4437-b9c0-50b75a47b8d7)

And another screenshot to showcase the user being a member of users.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/ac4a4e81-243d-491c-802f-b2b13133f680)

## Logon with User Account
Next, I logged into the account I created, which can be seen below.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/5627518f-1a61-4421-a3cd-cecb46068ba3)

## Automated AD Administration
### Change Powershell Permissions
The execution policy in Powershell serves as a security safeguard, regulating when Powershell loads files and executes scripts.
As a team, we decided to change the CurrentUser execution policy from Undefined to RemoteSigned. 
We did this by using the -SetExecutionPolicy command and then by specifying which policy we wanted to change.
The lines of code we used as well as the list showcasing the change can be seen in the screenshot below.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/b8cbcf68-d35c-4040-9d1d-d59b5d28b1ea)

### Test Powershell Script Execution
To test the execution policy I had modified, I created a short script that fetches the current execution policy,
examines whether the execution policy is configured as RemoteSigned, then delivers a message depending on whether the policy is configured as RemoteSigned or not.
The execution of this script is seen below, and the script itself can be found in the .txt file submitted to my HW4 folder on GitHub.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/2cb67664-80f6-4c06-8e09-233a89574268)

### Create More AD Objects

In this section of the lab, we explored the Badblood repo, which adds lots of tools and objects to active directory domains. These tools are used to further understand and secure these domains. 
From the Github for Badblood, I downloaded the code for all of the content found in the repo.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/e3704e3c-61c6-4e50-a609-a3148e9abb01)

In Powershell, I then cd'ed into the directory where the .ps1 file was then executed the file. Upon running the file,  many different objects were downloaded, resulting in numerous screens like the one shown below.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/23184671-da45-4dcb-96cf-d7702d4146c8)

Unfortunately, one of the packages being downloaded wasn't making any progress, so I could not continue further with running the files. Below is a screenshot of the package downloading screen I had for about 20 minutes.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/ef237c64-dc26-4a72-8dad-adde8dade402)


