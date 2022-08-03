# **Network Forensic Analysis Report**


## **Time Thieves**

You must inspect your traffic capture to answer the following questions:



<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image1.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](Images/traffic_capture.png "image_tooltip")




1. What is the domain name of the users' custom site? frank-n-ted.com
2. What is the IP address of the Domain Controller (DC) of the AD network? 10.6.12.12
3. What is the name of the malware downloaded to the 10.6.12.203 machine? june11.dll
    * Once you have found the file, export it to your Kali machine's desktop. 
4. Upload the file to[ VirusTotal.com](https://www.virustotal.com/gui/).
5. What kind of malware is this classified as? Looks like a Trojan mostly



![alt_text](Images/virus_total_results.png "Virus Total Results")

---


## 


## **Vulnerable Windows Machine**



1. Find the following information about the infected Windows machine:
    * Host name ROTTERDAM-PC
    * IP address 172.16.4.4
    * MAC address 00:59:07:b0:63:a4  
![alt_text](Images/Rotterdam-PC.png "ROTTERDAM-PC")  

  
2. What is the username of the Windows user whose computer is infected?  
This website offered Windows user account from from Kerberos traffic  https://unit42.paloaltonetworks.com/using-wireshark-identifying-hosts-and-users/  
So, the username is: matthijs.devries
![alt_text](Images/UserName-Capture.PNG "User Name Capture")

3. What are the IP addresses used in the actual infection traffic?  
	185.243.115.84  
![alt_text](Images/IPaddresses.png "IP Addresses")

4. As a bonus, retrieve the desktop background of the Windows host.  
Hackertarget.com gives a cheetsheet on finding an image, There were only a few files that were worth considering because of the size of the files. This one actually looks like a screenshot of a desktop  
![alt_text](Images/image_location.png "Desktop Image Located")
![alt_text](Images/desktop_image.png "Desktop Image")


---


## 


## **Illegal Downloads**



1. Find the following information about the machine with IP address 10.0.0.201:  
    * MAC address 00:16:16:18:66:c8  
      ![alt_text](Images/MAC_address.png "MAC Address")
    * Windows username elmer.blanco  
      ![alt_text](Images/Username_find.PNG "User Name")
    * OS version Window NT 10.0  
      ![alt_text](Images/OS_Version.PNG "OS Version")  
      
2. Which torrent file did the user download?  
    * Betty_Boop_Rhythm_on_the_Reservation.avi.torrent  
      ![alt_text](Images/BettyBoop.PNG "Torrent File")  
