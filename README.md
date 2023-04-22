# VAPT on existing website using OWASP tool

![image](https://user-images.githubusercontent.com/110705457/233799405-c8478194-8588-4d54-b4b4-ff8d9eccc015.png)

***INTRODUCTION***

Penetration testing or Pen Test is the most commonly used security testing technique for web applications.

Website penetration testing is a simulated hacker-style attack on a website aimed at identifying and gauging the gravity of existing vulnerabilities in order to protect the website from malicious attacks. This is to say, Penetration Testing focuses more on how each of these vulnerabilities could be exploited as opposed to Vulnerability Assessment, which merely identifies and lists all existing vulnerabilities in your website.

***IMPLEMENTATION***

•	METASPLOIT Framework:

Metasploit is simple to use and is designed with ease-of-use in mind to aid Penetration Testers.
Metasploit Framework follows these common steps while exploiting any target system

1.	Select and configure the exploit to be targeted. This is the code that will be targeted toward a system with the intention of taking advantage of a defect in the software. Validate whether the chosen system is susceptible to the chosen exploit.
2.	Lect and configure a payload that will be used. This payload represents the code that will be run on a system after a loop-hole has been found in the system and an entry point is set.
3.	Select and configure the encoding schema to be used to make sure that the payload can evade Intrusion Detection Systems with ease.
 
•	OWASP ZAP tool:

Zed Attack Proxy (ZAP) is a free, open-source penetration testing tool being maintained under the umbrella of the Open Web Application Security Project (OWASP). ZAP is designed specifically for testing web applications and is both flexible and extensible.

At its core, ZAP is what is known as a “man-in-the-middle proxy.” It stands between the tester’s browser and the web application so that it can intercept and inspect messages sent between browser and web application, modify the contents if needed, and then forward those packets on to the destination. It can be used as a stand-alone application, and as a daemon process.

![image](https://user-images.githubusercontent.com/110705457/233799635-99e5d93c-e3b2-45d0-904f-3e8bef4a739e.png)

ZAP provides functionality for a range of skill levels – from developers, to testers new to security testing, to security testing specialists. ZAP has versions for each major OS and Docker, so you are not tied to a single OS. Because ZAP is open-source, the source code can be examined to see exactly how the functionality is implemented. Anyone can volunteer to work on ZAP, fix bugs, add features, create pull requests to pull fixes into the project, and author add-ons to support specialized situations.

***RESULTS***

> Running web application server using Metasploit framework
<img src="https://user-images.githubusercontent.com/110705457/233799712-1a11237b-851e-4f1a-b86a-0650bf7d7284.png" width="800">

>When we enter $ifconfig command, we can see that the IP address obtained is 192.168.30.132
<img src="https://user-images.githubusercontent.com/110705457/233799737-fd74ccb5-602c-496b-858e-d7279a99274c.png" width="800">

>We will go and enter the obtained IP address in Firefox browser of Kali Linux. We can go into mutillidae which is born to be hacked website meant for hacking
<img src="https://user-images.githubusercontent.com/110705457/233799754-28c49883-7f3c-4695-9f14-8ecaa263e1c3.png" width="800">

>Copy browser link of the below screenshot which is obtained when clicked on OWASP Top 10  A2 Cross Site Scripting (XSS)  Via “Input” (GET/POST)  Add to your blog
<img src="https://user-images.githubusercontent.com/110705457/233799773-3b28efd4-a1cd-47d3-805f-b00f8af265ad.png" width="800">

>Run OWASP-ZAP in the Kali Linux terminal
<img src="![image](https://user-images.githubusercontent.com/110705457/233799792-df3ca11b-4508-4bc4-acc1-f62759867ce6.png)
" width="800">

>Persisting a Session
<img src="https://user-images.githubusercontent.com/110705457/233799807-018ae5b4-1f44-45fd-9427-31820922de99.png" width="800">

>Running an Automated Scan
<img src="https://user-images.githubusercontent.com/110705457/233799829-bb9bedca-b0e8-4730-87d0-523b774622e0.png" width="800">

>View Alerts and Alert details
<img src="https://user-images.githubusercontent.com/110705457/233799858-44432ec8-26c3-4aca-9e54-eb57f5b3da3b.png" width="800">

>Exploit through the link obtained in path traversal
<img src="https://user-images.githubusercontent.com/110705457/233799879-ea795e4d-5dd4-42b1-a906-aaaaa0e8b2e9.png" width="800">

***CONCLUSION***

Unlike the “old school” applications, web applications offer a lot to the market in terms of commerciality and usefulness. They bring functionality to the internet but for a cost. These systems are usually publicly available and hence exposed to the internet at all times. Because of the growing popularity and presence on the internet, web applications usually carry vulnerabilities in their design and configuration which malicious hackers find and exploit. Since these systems are almost always internet facing, they carry a greater risk with them and should automatically be a priority when it comes to penetration testing.

If the application handles some credit card data, personal information or even health records, it would be in a company’s best interest to perform annual web application penetration testing in order to meet regulatory compliance that most of the data requires. In cases where penetration testing is not required, it is highly recommended as the best mean to meet the best security standards, then to avoid performing it. With varying tools to choose from, web application penetration testing has developed a much more structured approach to automated and manual testing. Choosing any open-source security solutions is highly recommended with the availability of commercial versions of the same tool with upgraded capabilities.

To end with, web application penetration testing involves testing the application’s environment, database connectivity, source code, bad data and error data in order to find vulnerabilities and exploit them.



