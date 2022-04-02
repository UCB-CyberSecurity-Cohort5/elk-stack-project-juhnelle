## Activity File: Exploring Kibana

* You are a DevOps professional and have set up monitoring for one of your web servers. You are collecting all sorts of web log data and it is your job to review the data regularly to make sure everything is running smoothly. 

* Today, you notice something strange in the logs and you want to take a closer look.

* Your task: Explore the web server logs to see if there's anything unusual. Specifically, you will:

:warning: **Heads Up**: These sample logs are specific to the time you view them. As such, your answers will be different from the answers provided in the solution file. 

---

### Instructions

1. Add the sample web log data to Kibana.

2. Answer the following questions:

    - In the last 7 days, how many unique visitors were located in India?
    In the last 7 days, there were 244 unique visitors located in India.
  
  
  Unique Visitors in India.png
  
  
  
    - In the last 24 hours, of the visitors from China, how many were using Mac OSX?
In the last 24 hours, 63 visitors from China were using Mac OSX

    - In the last 2 days, what percentage of visitors received 404 errors? How about 503 errors?
    In the last 2 days, 7.143% of visitors received a 404 error and 2.857% of visitors received a 503 error.
    - In the last 7 days, what country produced the majority of the traffic on the website?
    China produced the majority of traffic on the website in the last 7 days.
    - Of the traffic that's coming from that country, what time of day had the highest amount of activity?
    13:00 was the time of day that had the highest amount of activity in China.
    - List all the types of downloaded files that have been identified for the last 7 days, along with a short description of each file type (use Google if you aren't sure about a particular file type).
Types of downloaded files in the last 7 days:
gz:  Will compress a file using gzip
css: Will format the contents of a webpage using HTML
deb: Unix archive files used to install packages on a linux OS
rpm: This file stores installation packages 

3. Now that you have a feel for the data, Let's dive a bit deeper. Look at the chart that shows Unique Visitors Vs. Average Bytes.
     - Locate the time frame in the last 7 days with the most amount of bytes (activity).
     - In your own words, is there anything that seems potentially strange about this activity?
     The chart shows that an average of  9,367 bytes were used on 3/23/2022, which is strange considering that it is such a high amount of bytes for just one user.


4. Filter the data by this event.
     - What is the timestamp for this event?
     The timestamp for this event is 2022-03-23 at 17:00:00.
     - What kind of file was downloaded?
     The type of file downloaded during this time was a deb file.
     - From what country did this activity originate?
     This activity originated from the USA.

     - What HTTP response codes were encountered by this visitor?
     The user encountered 202 HTTP response codes.


5. Switch to the Kibana Discover page to see more details about this activity.
     - What is the source IP address of this activity?
     The source IP of this activity is 234.226.50.122

     - What are the geo coordinates of this activity?
     The geo coordinates of this activity are: {  "lat": 46.94100778,"lon": -98.01762611}

     - What OS was the source machine running?
     The source machine was running Windows xp

     - What is the full URL that was accessed?
     The full url that was accessed was https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-6.3.2.deb
as accessed?
     
     - From what website did the visitor's traffic originate?
     The user’s traffic originated from http://nytimes.com/success/gerald-p-carr


6. Finish your investigation with a short overview of your insights. 

     - What do you think the user was doing?
     It seems that the user was trying to download a deb file from the website.

     - Was the file they downloaded malicious? If not, what is the file used for?
      Deb files can potentially be malicious, but not always. Deb files are used to install packages on a Unix OS.

     - Is there anything that seems suspicious about this activity?
     It is suspicious how the user was redirected by the nytimes website to download this deb file and the amount of bytes it required.

---
© 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.  
