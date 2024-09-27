<h1>Investigating Incidents with Splunk</h1>


<h2>Project description</h2>
For this project, I acted as a Cybersecurity Analyst on a security team for an organization. One of my job roles involved searching Splunk for incident information. This was based on the Improving Incident Response with Accountability Task in the Logging for Accountability Room from the TryHackMe.com website.<br/><br/>

<h2>Language and Applications</h2>

- <b>Splunk</b></br></br>

<h2>Environments Used </h2>

- <b>TryHackMe.com</b></br></br>

<h2>Project Walkthrough</h2>

<h3>1. How many total events are indexed by Splunk?</h3>

First, I began by logging into the Splunk Enterprise website for the organization and selecting 'Search & Reporting.'</br></br>
                                                
<p align="center">
<img src="https://i.imgur.com/OWUj3JX.png" height="80%" width="80%" alt="Empty Splunk search box"/>
<br />
<br />
</p>

In the search bar, I typed 'index=\*' This means that I want to retrieve all index records. The '\*' is a wildcard character.</br></br>

<p align="center">
<img src="https://i.imgur.com/eLruspo.png" height="80%" width="80%" alt="Empty Splunk search box"/>
<br />
<br />
</p>

On the right side of the search bar are the search filters. I set the search filter to 'All time.'</br></br>

<p align="center">
<img src="https://i.imgur.com/NrR9liC.png" height="80%" width="80%" alt="Empty Splunk search box"/>
<br />
<br />
</p>

The next thing I did was click on the magnifying glass button to initiate a search. I noted that 12,256 events were returned by the search.</br></br>

<p align="center">
<img src="https://i.imgur.com/vDHOxKQ.png" height="80%" width="80%" alt="Empty Splunk search box"/>
<br />
<br />
</p>

<h3>2. How many events were indexed from April 15th to 16th 2022?</h3>

For this question, I modified the search filter and set it to a specific date range.</br></br>
                                                
<p align="center">
<img src="https://i.imgur.com/qzXfBTR.png" height="80%" width="80%" alt="Open the file that contains the allow list"/>
<br />
<br />
</p>

After clicking the 'Apply' button and the magnifying glass button, the system returned the following results. I noted that 12,250 events were returned by the search.</br></br>

<p align="center">
<img src="https://i.imgur.com/ESa2Gqh.png" height="80%" width="80%" alt="Open the file that contains the allow list"/>
<br />
<br />
</p>

<h3>3. How many unique users appear in the data set?</h3>

On the left side of the Search, under SELECTED FIELDS, I noted that 4 users were returned by the search.</br></br>
                                                
<p align="center">
<img src="https://i.imgur.com/IgNnC3g.png" height="40%" width="40%" alt="Open the file that contains the allow list"/>
<br />
<br />
</p>

<h3>4. How many events are associated with the user "James"?</h3>

Again, on the left side of the Search, under SELECTED FIELDS, I clicked on the 'User' link. This opened up search results based on individual users. I noted that the user account for James was associated with 5 events.</br></br> 

<p align="center">
<img src="https://i.imgur.com/QHlT8R2.png" height="80%" width="80%" alt="Read the file contents"/>
<br />
<br />
</p>

<h3>5.What utility was used in the oldest event associated with "James"?</h3>

After selecting James' name and scrolling down to the last event, I used the find function in my browser to discover that the utility was 'WMI Commandline,' which is wmic.exe.<br/><br/>

<p align="center">
<img src="https://i.imgur.com/k7qWfH4.png" height="100%" width="100%" alt="Convert the string into a list"/>
<br />
<br />
</p>

<h3>6. What event ID followed process creation events associated with "James"?</h3>

The event that occurred after the Process Create events was the newest event in the search results. I noted that the event ID was 3.<br/><br/>

<p align="center">
<img src="https://i.imgur.com/813I0ou.png" height="60%" width="60%" alt="Iterate through the IP addresses list"/>
<br />
<br />
</p>

<h3>Summary</h3>

In this exercise, I demonstrated the use of Splunk to search for incident information as a cybersecurity analyst. This example displayed how effective Splunk can be as a SIEM tool for retrieving the correct information for incident response.


