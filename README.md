# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:bookmyshow.com" would search for pages that are on the example.com domain.



![Screenshot 2025-03-14 143055](https://github.com/user-attachments/assets/0b611f92-cbab-48e4-8447-ee067cc45fd9)


Following searches for all the sites that is in the domain yahoo.com

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

<img width="944" alt="image" src="https://github.com/user-attachments/assets/d92e5fbe-c150-4601-b828-cd8ee90e95c4" />




intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

<img width="926" alt="image" src="https://github.com/user-attachments/assets/2154ecce-be6a-439b-9a8f-9b2c84df5bdc" />



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

<img width="929" alt="image" src="https://github.com/user-attachments/assets/c60b4ea6-053c-45f2-b4e5-07d1e12a1135" />


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

<img width="937" alt="image" src="https://github.com/user-attachments/assets/804eb155-22c1-476a-8d88-9d4df5fcbc37" />


link: This operator allows you to search for pages that link to a specific URL. For example, "link:bookmyshow.com" would search for pages that link to the example.com domain.
### Output:
<img width="941" alt="image" src="https://github.com/user-attachments/assets/5c2c1d03-f15e-4c53-8734-f8b7554542a3" />

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
### Output:

<img width="959" alt="image" src="https://github.com/user-attachments/assets/581b9c1e-a0d3-445b-849d-4abe4d85c946" />



 
# DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

<img width="411" alt="image" src="https://github.com/user-attachments/assets/fe06203f-c782-431a-b599-e339ac70874b" />

<img width="419" alt="image" src="https://github.com/user-attachments/assets/6ddf4e65-3f13-43ee-8e01-36029b22f8df" />






## dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.

### Output:

<img width="424" alt="image" src="https://github.com/user-attachments/assets/22a2d7fc-5b3b-471a-aacb-f0ebdd57abe7" />


## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

## Output:

<img width="470" alt="image" src="https://github.com/user-attachments/assets/73a6ebbe-14c5-43f2-bddf-3185dc802c9d" />



# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output

 <img width="292" alt="image" src="https://github.com/user-attachments/assets/fd9a067f-8220-44d2-a0e5-4e5865cc3396" />

  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

<img width="434" alt="image" src="https://github.com/user-attachments/assets/eabef1d5-a29f-4b1c-ac06-7044af04cf4d" />



## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

