# Areas of Defensive Security
## Security Operations Center (SOC)
* Focuses on network monitoring to detect malicious activity
	* Vulerabilities
	* Policy Violations
	* Unauthorised activity
	* Network intrusions

## Threat Intelligence
Knowledge is power. Threat Intelligence is all about using the threat information at hand to create/reinforce a better defense.

## Digital Forensics and Incident Response (DFIR)
* Primarily focus on analysing the evidence of a security breach

### Incident Response (IR)
* Damage reduction by getting in front of the document.
* Incident : ==Usually== refers to a cyber attack or data breach but can be something less critical such as a ==misconfiguration, intrusion attempt or policy violation== 
* Incident Response is all about the methodology used to respond to a particular event
	* Aim is to minimise damage and maximise recovery time

		#### Four phases of IR:
		![Incident Response chain | 800](https://tryhackme-images.s3.amazonaws.com/user-uploads/5f04259cf9bf5b57aed2c476/room-content/3b16bdb89d8cec6982746da2a1369cf3.png)
### Malware Analysis
Two types:
1. Static: inspection of malicious programme ==without== running it
2. Dynamic: run malware in a controlled environment and observe how it runs


## Practical Example of Defensive Security
You are part of a _Security Operations Center_ (SOC) responsible for protecting a bank. This bank’s SOC uses a ==Security Information and Event Management_ (SIEM) system. A SIEM gathers security-related information and events from various sources and presents them via one system.== For instance, you would be notified if there is a failed login attempt or a login attempt from an unexpected geographic location. Moreover, with the advent of machine learning, a SIEM might detect unusual behavior, such as a user logging in at 3 AM when he usually logs in only during work hours.  

In this exercise, we will interact with a SIEM to monitor the different events on our network and systems in real-time. Some of the events are typical and harmless; others might require further intervention from us. Find the event flagged in red, take note of it, and click on it for further inspection.

Next, we want to learn more about the suspicious activity or event. The suspicious event might have been triggered by an event, such as a local user, a local computer, or a remote IP address. To send and receive postal mail, you need a physical address; similarly, you need an IP address to send and receive data over the Internet. An IP address is a logical address that allows you to communicate over the Internet. We inspect the cause of the trigger to confirm whether the event is indeed malicious. If it is malicious, we need to take due action, such as reporting to someone else in the SOC and blocking the IP address.