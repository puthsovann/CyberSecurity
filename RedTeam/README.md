# Cyber Kill Chain
It is an adaptation of the military’s kill chain, which is a step-by-step approach that identifies and stops enemy activity. Originally developed by Lockheed Martin in 2011, the cyber kill chain outlines the various stages of several common cyberattacks and, by extension, the points at which the information security team can prevent, detect or intercept attackers.

![KillChain](resouce/killchain.png)

## Reconnaissance
[More](1Recon) - The attacker gathers information on the target before the actual attack starts. He can do it by looking for publicly available information on the Internet.

## Weaponization
[More](2Weapon) - The attacker uses an exploit and creates a malicious payload to send to the victim. This step happens at the attacker side, without contact with the victim.

## Delivery
[More](3Delivery) - The attacker sends the malicious payload to the victim by email or other means, which represents one of many intrusion methods the attacker can use.

## Exploitation
[More](4Exploit) - The actual execution of the exploit, which is, again, relevant only when the attacker uses an exploit.

## Installation
[More](5Install) - Installing malware on the infected computer is relevant only if the attacker used malware as part of the attack, and even when there is malware involved, the installation is a point in time within a much more elaborate attack process that takes months to operate.

## Command and control
[More](6C2Server) - The attacker creates a command and control channel in order to continue to operate his internal assets remotely. This step is relatively generic and relevant throughout the attack, not only when malware is installed.

## Action on objectives
[More](7ActionOnObj) - The attacker performs the steps to achieve his actual goals inside the victim’s network. This is the elaborate active attack process that takes months, and thousands of small steps, in order to achieve.

## RedToolKit
![RedToolKit](resouce/RedToolKit.png)
