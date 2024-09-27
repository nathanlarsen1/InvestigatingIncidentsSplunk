<h1>Investigating Incidents with Splunk</h1>


<h2>Project description</h2>
For this project, I acted as a Cybersecurity Analyst on a security team for an organization. One of my job roles involved wiping a USB drive. I chose to use the diskpart command in Windows.<br/><br/>

<b>Warning: This is for educational purposes only.</b> Using this information to wipe drives can permanently erase valuable data. Proceed with extreme caution and at your own risk.<br/><br/>

<h2>Language and Applications</h2>

- <b>Command Prompt</b>
- <b>Diskpart</b></br></br>

<h2>Environments Used </h2>

- <b>Windows 11</b></br></br>

<h2>Project Walkthrough</h2>

<h3>1. Search for Command Prompt</h3>

I began by typing "Command Prompt" in the Windows search bar.</br></br>
                                                
<p align="center">
<img src="https://i.imgur.com/4tfaGs4.png" height="80%" width="80%" alt="Open the file that contains the allow list"/>
<br />
<br />
</p>

<h3>2. Right-click and Run as Administrator</h3>
Then I right-clicked on the "Command Prompt" result and selected "Run as administrator."</br></br>
                                                
<p align="center">
<img src="https://i.imgur.com/7bCi1DW.png" height="30%" width="30%" alt="Open the file that contains the allow list"/>
<br />
<br />
</p>

<h3>3. Command Prompt</h3>
The Command Prompt opened.</br></br>
                                                
<p align="center">
<img src="https://i.imgur.com/gxojtvH.png" height="80%" width="80%" alt="Open the file that contains the allow list"/>
<br />
<br />
</p>

<h3>4. Diskpart</h3>

In the command prompt, I typed `diskpart` and pressed Enter.</br></br> 

<p align="center">
<img src="https://i.imgur.com/TGhFnGl.png" height="80%" width="80%" alt="Read the file contents"/>
<br />
<br />
</p>

<h3>5.List Disk</h3>

After Dispart opened, I typed `list disk` and pressed Enter.<br/><br/>

<p align="center">
<img src="https://i.imgur.com/E8W9BR7.png" height="80%" width="80%" alt="Convert the string into a list"/>
<br />
<br />
</p>

<h3>6. List of Disks</h3>

A list displayed of all connected disks.<br/><br/>

<p align="center">
<img src="https://i.imgur.com/mxKdhnd.png" height="80%" width="80%" alt="Iterate through the IP addresses list"/>
<br />
<br />
</p>

<h3>7. Disk Number</h3>

I carefully reviewed the list and identified the disk that I needed to wipe. I typed `select disk 1` and pressed Enter.<br/><br/>

<p align="center">
<img src="https://i.imgur.com/TbdSwtf.png" height="80%" width="80%" alt="Remove IP addresses that are on the remove list"/>
<br />
<br />
</p>

<h3>8. Clean Command</h3>

Then in the diskpart prompt I entered `clean` and pressed Enter. I made sure that I had the correct disk before proceeding knowing that this process will permanently erase all data on the selected disk. This was done by double-checking the disk number before proceeding, as wiping the wrong disk can have irreversible consequences.<br/><br/>

<p align="center">
<img src="https://i.imgur.com/caTn1Ec.png" height="80%" width="80%" alt="Update the file with the revised list of IP addresses"/>
<br />
<br />
</p>

<h3>9. Dispart Succeeded</h3>

Once the process was finished, I saw a message indicating that Diskpart succeeded in cleaning the disk.</br></br>

<p align="center">
<img src="https://i.imgur.com/SpBLgP4.png" height="80%" width="80%" alt="Update the file with the revised list of IP addresses"/>
<br />
<br />
</p>

After I was finished, I typed `exit` to leave Diskpart and closed the Command Prompt window.</br></br>

<h3>Summary</h3>

In this excerise, I demonstrated the use of diskpart to wipe a drive as a Cybersecurity Analyst. This example displayed how drives can easily be wiped for reuse.


