# Reconnaissance (Information Gathering)

## 1st CLASS about Ethical Hacking
#

<u><b>Topics</b></u>

+ What is information Gathering/ Footprinting/
+ Which information we gather
+ Types of information gathering
+ How we gather information
+ Reverse image search
+ Google hacking database


## Recon / Information Gathering / Footprint /
+ Information Gathering is Collecting data about some network/host/system.
+ Footprinting => Footstep + printing(logging)
 
## Types of information gathering
+ Based on how we do the recon
    1. Active Footprinting
    2. Passive Footprinting

1. Active Footprinting
This kind is when we try to gather information directly by contacting that person.

Example:
+ When you go to the bank and ask for some informations.
+ Chatting with person on social media to know about them.

2. Passive Footprinting
This kind of recon is when you gather informations from another person,3rd party or by checking public sources.

Example:
+ To know the bank working time i can see the posted texts.
+ To know someone name by reading the username.

## What type of information do you gather?
### a. Host
+ Websites
+ Computers
+ Smart Phone
### b. Network
+ Home Network
+ Companie networks
### c. Person/Organization
### d. Application

#
## A. Websites
+ The informations we gather about a websites are
    + IP Addresses
    + Development frameworks
+ Web server version.
+ Technologies used
    + Name
    + Domain registrations

+ To get ip
    + To get ip address of some website:
        + Active recon
           + ping website_link

                 ping moe.gov.et

           + nslookup website_link
                
                 nslookup moe.gov.et

+ Passive recon
    + www.nslookup.io

+ To get development frameworks
    + Wapplyzer
    + Terminal tool
    + whatweb

+ To get the name
    + You can see the title of the website or texts inside the page also the url.
+ Details about domains
+ you can use whois terminal +website tool
    + sudo apt install whois
    + who.is

## B. Computers/Phone
+ The informations we gather about a Computers/Hosts are
    + IP Addresses
    + OS informations
    + HostName
    + MAC address
    + Open services or ports
## C. Networks
+ The informations we gather about a Networks are
    + IP Addresses
    + Ports,Services
    + Class and Type of Network
    + Hosts on that Network
    + Strength and security of that Network

## D. Personal Informations
+ he informations we gather about a Persons are
    + Full Name
    + Address
+ Physical Address
+ All Social Media Address
+ Phone address
+ What the person loves
+ Job
+ Friends
+ Status
+ skills
## E. Applications/Softwares
+ The informations we gather about a Applications are
    + What they are made up of
+ Which programming language used
+ Which framework used

## Reverse image search
+ Reverse image search is a technique of searching with images.
+ We all search with text but we can search with images to This can give as more information
+ Ex: think like user posted a picture with a background of some area, if the user didnt talk about the place we can just search the image and the search engines will give as some similar photos where they are taken in same place(not 100% accurate)

We can use:
+ https://tineye.com/
+ https://www.labnol.org/reverse/
+ https://images.google.com/


## Google Dorking(Google Hacking Database)
+ it's not hacking into Google servers!
+ Google hacking is using different Google operators to effectively optimize search results.
+ It also involves using Google to identify vulnerabilities in websites.
+ Results are highly customizable.

👉 THIS IS THE MOST POWERFUL SKILL OF HACKER!

## Basic operators
+ For inclusion of something common (+)
    + Nathan Hailu +geeztech +ceo
+ Terms you want to exclude (-)
    + Anti-virus -software
    + Georgia -america -state
+ Search for an exact term (“)
    + “How to eat food”
    + “Nathan Hailu” 
+ ( * ) any word (wild card)
○ It tells Google to try to treat the star as a placeholder for any unknown term(s) and then find the best matches.
    + Estonia parliament voted on the * bill
+ ( | ) boolean ‘OR’
    + “Nathan Hailu” | “Natan Hailu”

## Advanced Operators
+ These are Syntaxes used by Google.
    + intitle
        + Google returns results with the word/phrase found within the
title of the page
            + intitle:index.of
    + inurl
        + Finds a specific term within the URL
            + inurl:view/index.shtml
    + filetype
        + Searches for a specific filetype
            + “Hacking” filetype:pdf
            + filetype:txt
    + Intext
        + Google returns links that contains Texts from that link
            + intext:”Hackers in Ethiopia

## Mixing Operators
+ Inurl:securethiscompany.com intitle:index.of
+ "mysql dump" Inurl: filetype:sql intext:password
+ inurl:ftp "password" filetype:xls
+ intitle:admin intitle:login
+ intitle:phpMyAdmin “Welcome to phpMyAdmin ***” “running on * as root@*”