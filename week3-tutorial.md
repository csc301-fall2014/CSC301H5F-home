CSC301 Tutorial 3 – Section 1 
Proposal: Build a system that detects and reports power usage (in home or office).
Initial Discussion:
What is the system is going to detect?
•	Appliances – fridge, washing machine, dishwasher
•	Electronics – computers, TV, microwave
•	Air conditioning or heating system
•	Lights 

Where/How will you display the information?
•	Computer/Mobile app
•	Online website/app
•	Hardware interface
•	TV channel
•	Smartwatch

Only statistics or intelligent optimization of power usage?
•	Depends on how you deliver the information.
•	Optimization will require complicated UI

Pricing?
•	Depends on how complicated the electricity detection is.

Personas:
John “The Family Man” Doe: John is 45 years old, but feels much older. He’s a plumber, his job is also his hobby (he experiments plumbing in his own house). He lives in two story townhouse with a big basement (with an office). He has fifteen children (from multiple mistresses) who are quite troublesome. This makes him cranky and he’s usually on a short fuse. He’s not tech savvy, and he wants to keep it on budget so he can save money to invest in his business. 

User Stories:
1.	John TFM Doe wants his lights to cost him less. He wants specific information on the usage of the lights in the house as well as the possibility of the system being able to turn them off so he doesn’t have to take money out of his kids’ college fund.  Priority: High, Difficulty: High
2.	John TFM Doe wants the system to alert him if his appliance’s power usage go over a set threshold so he knows when he is using them too much. Priority: Medium, Difficulty: Low
3.	John TFM Doe wants to know the area of the house that uses the most electricity, so he can identify which of his kids he should scold more often. Priority: Low, Difficulty: High


High-Level Architecture:
The hardware component of the system would involve smart plugs as well as “nodes” (that record usage) at places around the house. These plugs and nodes would need to be programmed to deliver information to a microcontroller (possibly an Arduino) that would display the necessary information.

First Iteration:
Obtain and install a node in a room (possibly John’s office) and program it to simply record daily usage. Connect it to an Arduino microcontroller and program it to display the usage at the end of a day. 


CSC301 Tutorial 3 – Section 2 
Proposal: Build a system that detects and reports power usage (in home or office).
Initial Discussion:
What platform are you going to see the reported data on?
•	Mobile/web application
•	Smartwatch
•	TV channel
•	Hardware 

What things are we going to get the data from?
•	Lights
•	Appliances
•	Electronics

What kind of features do you want (basic reporting or intelligent system)?
•	Basic for first iteration, with possibility of intelligent system (so build a robust system)

Personas:
Ted Mosby is a 30 year old single man. A failed architect, he now manages the bar under his apartment. He is neurotic and is usually drunk with his friends (who are troublesome and don’t respect his privacy). He wants to marry someone, but his power bill is so high he can’t afford to yet. He wants to figure out his power usage to conserve and save up for a wedding, after he meets the mother of his children. 

Sally “the babysitter” Drew is 24 year old single mom. She babysits a lot of kids (between 3-6 years old). She has a little boy (still a toddler). She is organized, she can cook well and she’s an aspiring musician (with a studio in the house). She likes creeping people on Facebook (especially ones she is jealous of). She wants her baby to grow up successful and she’s worried her high power bill will restrict that. 



User Stories:
Sally wants to make her studio cost effective, she uses it a lot and kids she babysits always turn things on, and leave them on. Priority: High, Difficulty: Medium

Sally wants to know how much she uses her computer (to creep on facebook) so she can motivate herself to use it less. Priority: High, Difficulty: Low

Sally wants the system to intelligently know which lights to turn off (if it detects someone leaving the room, or using a timer), which she believes would save her money. Priority: Low, Difficulty: High

High-Level Architecture:
The hardware component of the system would involve smart plugs as well as “nodes” (that record usage) at places around the house. These plugs and nodes would need to be programmed to interface with a wireless communication device (WiFi or Bluetooth), which could be connected to phone/PC. A computer/mobile application would analyze and display the power usage data, and would retain control of the system. 

First Iteration:
Obtain and install a smart plug (w/ Bluetooth transmit) on Sally’s computer and program it to record how long it is on. Using data on the computer as well as the data from the plug, notify Sally of her usage at the end of each day using a simple mobile application.
