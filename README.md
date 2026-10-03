# Help-Desk-Simulator
realistic IT tickets: investigate with real commands, find the root cause, apply the fix, and document the resolution.

About the project

I built this project to practice the day-to-day work of a Tier 1 help desk technician
Instead of memorizing answers, you have to gather evidence, reason through it, and document your work the way you would on the job.

Each ticket follows four steps:

1. Investigate. 
2. Identify the cause.
3. Apply the fix.
4. Document and close.

Wrong answers cost 15 points each and explain why they're wrong, so every mistake teaches something.

Ticket scenarios
Ticket	Scenario	A+ domain
INC-1001	Websites won't load, but pings to IPs work	Core 1: Network troubleshooting (DNS)
INC-1002	Print jobs stuck while printer shows Ready	Core 1: Printer troubleshooting
INC-1003	Locked-out user asks for a quick password reset	Core 2: Security and social engineering
INC-1004	Slow PC after downloading freeware	Core 2: Malware removal steps
INC-1005	New hire gets Access Denied on a file share	Core 2: NTFS/share permissions
INC-1006	"No bootable device" on startup	Core 1: Boot and storage troubleshooting
INC-1007	Blue screens after a driver update	Core 2: Windows OS troubleshooting
INC-1008	APIPA address after moving desks	Core 1: Network connectivity and VLANs
Skills demonstrated
Using the CompTIA A+ troubleshooting methodology
Diagnosing network problems (DNS, DHCP/APIPA, VLANs)
Managing Windows services, drivers, and boot settings
Following security practices: identity verification, least privilege, and the malware removal process
Writing clear ticket documentation and knowing when to escalate
Front-end development in HTML, CSS, and JavaScript
How to run it

No installation needed.

Online: open the live demo.
Locally: download index.html and open it in any modern browser.

Progress saves in your browser automatically. To start over, click Reset progress twice.

Adding your own tickets


<h2> Network troubleshooting (DNS)</h2>

![image](https://github.com/Harrowtheegreat/Help-Desk-Simulator/blob/b88c60efeaa93fec0455a0028383b87e2f7304f4/Screenshot%202026-09-27%20113343.png)

<h2> Ticket 1 </h2>

Websites won't load, but pings to IPs work

I used all three diagnostic tools (ipconfig, nslookup, icacls, which are commands that you can use  
to identify network issues.

![image](https://github.com/Harrowtheegreat/Help-Desk-Simulator/blob/23655a2f4d656ef14f5ae99dc7b6c28aab265306/Screenshot%202026-09-27%20113908.png)



The DNS server setting points to the address that doesn't respond 

this  means your computer is set to ask a specific server to translate website names (like google.com) into IP addresses, but that server isn't answering. So the computer can't find websites by name, even though the network connection itself may be fine.
![image](https://github.com/Harrowtheegreat/Help-Desk-Simulator/blob/1ab48baa3f891df4174c1b3d77d550aeb9cc2bc9/Screenshot%202026-09-27%20114206.png)


Now its  time to apply the FIX
Now by Setting DNS back to automatic lets DHCP hand out the correct company DNS server, and flushing clears out any bad cached lookups.

Setting DNS to automatic lets DHCP assign the company's correct DNS server. A wrong manually set DNS can block access to internal sites, shared drives, and company resources. Automatic settings also stay up to date if the network changes.

Flushing the DNS cache clears out old or incorrect saved lookups. Without it, the computer may keep using bad addresses even after the settings are fixed.

Together, these steps make sure the computer finds the right servers and the fix takes effect immediately.

![image](https://github.com/Harrowtheegreat/Help-Desk-Simulator/blob/a84a05a6d7d7dfdbdec75cfb3520f8d6324329be/Screenshot%202026-09-27%20114354.png)

Now in true helpdesk fashion we document our tickets then close them  
Documenting help desk tickets matters because it:


![image](https://github.com/Harrowtheegreat/Help-Desk-Simulator/blob/cafaacd17d1fd6cac4d8841080a5b565c873c58c/Screenshot%202026-09-27%20115832.png)


Documenting help desk tickets 


Saves time: If the same issue comes up again, the fix is already written down.
Keeps everyone informed: Anyone on the team can pick up a ticket and see what's been tried.
Shows patterns: Recurring problems become visible so root causes can be fixed.
Provides accountability: There's a clear record of who did what and when.
Builds a knowledge base: Past tickets become guides for training and self-service.
Improves the customer experience: Users don't have to repeat themselves.

![image](https://github.com/Harrowtheegreat/Help-Desk-Simulator/blob/0fe853daac829685f53e61fc037f3cb617ca3404/Screenshot%202026-09-27%20120239.png)

