# 1/c Faith Arnold - CNS Homework #3 - 13 September 2023 
## Red Hat Enterprise Linux 8
For this lab, I used the Red Hat Enterprise Linux 8 (RHEL 8) distribution. RHEL 8 provides a reliable environment for companies to test their software for performance and security. It is compatible with several different software packages and is equipped with tons of security features to use on a SCC infrastructure.
## Installing SCC
To find the SCC tool compatible with RHEL 8, I searched the Document Library on the cyber exchange website and used "SCC 5.7.2 RHEL 8/Oracle Linux 8 x86 64."

Before insalling the SCC itself, I first installed dependencies so that the SCC can run using the following command.
![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/5006f0b1-84b1-47f7-a131-a947eafefdb4)

Then, I went into the directory inside the SCC file where the .rpm file was, then ran the following command.
![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/9d359f1b-b756-428a-83ad-4d296c5eb8a3)

This launched the SCC GUI; I then started a scan of the system, which can be seen below.
![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/5aa026be-593d-48ff-8fd2-5f977732ce1e)

The scan summary shows a score of 36.36.
![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/e6f69d83-5b39-4b5b-a446-a1b363200d11)

Overall, 84 passed and 147 failed; in this scan, there were 21 CAT I checks.
![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/800c3bdd-0b8f-47d2-8ae7-f80e91171124)

