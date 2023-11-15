# 1/c Faith Arnold - CNS Homework #8 - 14 November 2023
## Research a Security Tool

For this homework, I chose Masscan as my tool. Masscan is a quick, open-source network scanning tool known for its speed in mapping large IP address ranges. Masscan employs asynchronous scanning, allowing it to send multiple packets simultaneously and complete scans of the entire IPv4 space in a short period of time. This speed makes it a great tool for network mapping, offering administrators swift insights into open ports across extensive address ranges. Masscan can be found on its GitHub repo at this link: https://github.com/robertdavidgraham/masscan

While Masscan excels at quickly identifying open ports, its focus on speed comes at the expense of detailed service information. The tool outputs results in raw formats, necessitating additional processing for human-readable interpretations. Unlike Nmap, Masscan lacks a scripting engine for advanced functions such as service version detection and vulnerability scanning. Despite its lack of detail, Masscan remains a top choice for situations demanding high-speed, large-scale network reconnaissance. Masscan can even be used to scan the entire Internet, averaging scans of an entire port taking 10 hours, though scanning the entire Internet is not recommended.

I installed Masscan on my Parrot OS using the command in the below screenshot.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/4d779c42-f4fb-4379-ab82-96121a5383b8)


## Demonstrate Use of the Chosen Tool

To use the tool, I conducted a scan on our .205 network, which is the target host used for the Lab 11 Splunk and Zeek interactions. The scan's results can be seen in the screenshot below.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/79cbe3ce-428f-473f-bf4f-7b93579834ee)

