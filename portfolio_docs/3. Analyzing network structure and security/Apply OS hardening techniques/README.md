## Overview
```
I take on the role of a cybersecurity analyst working for
a company that hosts the cooking website, yummyrecipesforme.com.

Visitors to the website experience a security issue when loading the main webpage.

Thus, my job is to investigate, identify, document, and recommend a solution to the security problem.

When investigating the security event, I will review a tcpdump log.
```

## Task
```
Writing an incident report for this security event
```

## Description
```
I am a cybersecurity analyst for yummyrecipesforme.com, a
website that sells recipes and cookbooks. A former employee has
decided to lure users to a fake website with malware.
The baker executed a brute force attack to gain access to the web host.
They repeatedly entered several known default passwords for the
administrative account until they correctly guessed the right one.
After they obtained the login credentials, they were able to access
the admin panel and change the website’s source code. They embedded
a javascript function in the source code that prompted visitors to
download and run a file upon visiting the website. After embedding
the malware, the baker changed the password to the administrative account.
When customers download the file, they are redirected to a fake version
of the website that contains the malware.
Several hours after the attack, multiple customers emailed yummyrecipesforme’s helpdesk.
They complained that the company’s website had prompted them to download a file to
access free recipes. The customers claimed that, after running the file,
the address of the website changed and their personal computers began running more slowly.
In response to this incident, the website owner tries to log in to the admin panel
but is unable to, so they reach out to the website hosting provider.
```

## Analyze Log
```
Used sandbox environment and tcpump nalyzer

1. The browser initiates a DNS request: It requests the IP address
of the yummyrecipesforme.com URL from the DNS server.
2. The DNS replies with the correct IP address. 
3. The browser initiates an HTTP request: It requests the yummyrecipesforme.com
webpage using the IP address sent by the DNS server.
4. The browser initiates the download of the malware.
5. The browser initiates a DNS request for greatrecipesforme.com.
6. The DNS server responds with the IP address for greatrecipesforme.com.
7. The browser initiates an HTTP request to the IP address for greatrecipesforme.com.
```

## Confirm the website was compromised
```
The analyst checks the source code for the website.
They notice that javascript code had been added to prompt
website visitors to download an executable file. Analysis of
the downloaded file found a script that redirects the visitors’
browsers from yummyrecipesforme.com to greatrecipesforme.com.
```


