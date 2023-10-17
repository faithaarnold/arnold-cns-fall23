# 1/c Faith Arnold - CNS Homework #5 - 03 October 2023
## Learning More About SSH

The following four screenshots are from the assigned RedHat Academy guided exercises.

10.2 #6

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/e53f877a-afb5-4da9-aad8-ae3a50d375f9)

10.2 #12

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/a5fa0087-2ce7-46c6-966c-04bb57db49f1)

10.4 #4

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/72ce19c2-4af0-4a17-9b95-fc0bca1496c1)

10.4 #9

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/9ade4a0c-10a7-437e-b7b0-807a70bff490)

## Applying Key Based Authentication

In this section of the homework, I logged into my domain user account on the NUC to generate an SSH key to loginto the jumpbox created for Lab 6. 

I generated a key by using the command "ssh-keygen."

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/7194999e-d2ba-498e-8256-885cc59d63bf)

Next, I needed to copy the contents of the public key into the jumpbox. I accomplished this by displaying the contents of the key using "cat" and copying those contents into my clipboard.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/e47dd52b-cc6a-4061-801b-b7f7f072ddd2)

After logging into the jumpbox, I used the nano text editor to paste the public key into the jumpbox. This allowed me to log into the jumpbox without being prompoted for a password, utilizing key based authentication. Both of these steps can be seen in the image below.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/eac35f92-6dd3-4f7a-9138-c2be91d13771)

## Brute Forcing Passwords

Logging into the jumpbox again, I changed my password using the "passwd" command to one from the list of passwords given in the "worst-passwords-2017-top100-slashdata.txt" from the SecLists repository. I chose "password" as my new password.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/9f3f17b4-f2dd-4481-9b52-d45704bd0b1c)

I then created two .txt files within my directory, the first being a user.txt file containing a list of usernames, one of them being the username used to login to the jumpbox. The second was a pass.txt file with the passwords from the "worst-passwords-2017-top100-slashdata.txt" list. 

Using nmap to brute force the password to the jumpbox, I ran the following command in powershell to begin the script.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/169d4403-8872-4b3a-bacc-3e66f7d9acee)

Below is a screenshot of the end of the script where the correct credentials were found.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/cb9512e2-42ad-425b-97e8-d61665e05242)
