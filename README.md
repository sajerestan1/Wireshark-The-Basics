# Wireshark-The-Basics

![image](https://github.com/user-attachments/assets/df25d19c-82a6-4f86-b89d-0de1325fc57e)

Personal Project: Packet Capture Analysis Using Wireshark
Scenario:

In this project, I was tasked with analyzing network traffic using Wireshark to investigate captured packets and extract specific information related to various protocols. The investigation required dissecting packet details, navigating capture files, and using filters to understand the underlying data structures and communication methods. This report details my process in answering the questions provided in this exercise.

### Task 1: Introduction

  1. Which file is used to simulate the screenshots?

     Answer: http1.pcapng

  I started by loading the necessary files for this task. The file http1.pcapng was identified as the file used to simulate the screenshots for this exercise.

  2. Which file is used to answer the questions?

     Answer: Exercise.pcapng



  The second file, Exercise.pcapng, was the primary file I used to answer the questions throughout this task.

### Task 2: Tool Overview

  #### What is the flag?
        
  Answer: TryHackMe_Wireshark_Demo

  To obtain this, I read the capture file comments found within the Exercise.pcapng file. The flag was explicitly mentioned in the comments section.

![image](https://github.com/user-attachments/assets/819a2bc5-f3a1-436f-ad9a-b8bc1edfc021)


![image](https://github.com/user-attachments/assets/f31fe0c7-4f40-4e3a-b7cf-1a80293ee98e)

#### What is the total number of packets?
  
  Answer: 58620

I opened the capture file properties dialog by navigating to the bottom left of the status bar in Wireshark, which displayed the total number of packets captured.

#### What is the SHA256 hash value of the capture file?

![image](https://github.com/user-attachments/assets/cbbc203a-d646-4ad0-8364-62cf9548b1cf)

Answer: f446de335565fb0b0ee5e5a3266703c778b2f3dfad7efeaeccb2da5641a6d6eb

The SHA256 hash of the file was displayed in the capture file properties section. This information can be verified by calculating the file hash using external tools or within Wireshark's properties dialog.

### Task 3: Packet Dissection

View packet number 38. Which markup language is used under the HTTP protocol?
        
  Answer: eXtensible Markup Language (XML)

![image](https://github.com/user-attachments/assets/a8a4fa97-e2b7-40b9-b9ac-536f2bc1719b)

Using Wireshark’s packet navigation feature (Ctrl + G), I navigated to packet number 38. Within the packet details pane under the HTTP protocol, I identified that XML was being used as the markup language.

![image](https://github.com/user-attachments/assets/ea567562-4647-4b07-9581-6d22f34908df)

### What is the arrival date of the packet?
        
  Answer: 05/13/2004

![image](https://github.com/user-attachments/assets/06f30619-ded3-47ea-80c1-ab62bf043225)

  In the Frame section of the packet details, I found the arrival date formatted as Month/Day/Year.

  ### What is the TTL value?
        
  Answer: 47

![image](https://github.com/user-attachments/assets/aef2327e-35e9-414c-a324-dc0bab6c91a9)

By expanding the Internet Protocol section within the packet details, I found the Time to Live (TTL) value listed as 47, which indicates how many hops the packet can traverse before being discarded.

### What is the TCP payload size?
       
  Answer: 424

  In the Transmission Control Protocol section (Layer 4), the TCP payload size was displayed as 424 bytes.

![image](https://github.com/user-attachments/assets/ce278593-c06e-40c8-9ab1-dac85de46317)

  What is the e-tag value?
        
  Answer: 9a01a-4696–7e354b00

  The e-tag value was located under the HTTP protocol section. The e-tag helps in identifying a specific version of a resource.

![image](https://github.com/user-attachments/assets/608c4fec-503e-4b1f-bbee-c292ebce045d)

Task 4: Packet Navigation

Search the "r4w" string in packet details. What is the name of artist 1?
        
  Answer: r4w8173

![image](https://github.com/user-attachments/assets/6234b59a-152d-45d3-bbde-f3de88b01a80)

  I used Wireshark’s search feature (Ctrl + F) to search for the string "r4w." This search led me to the details pane, where I identified the name of artist 1.

  Go to packet 12 and read the comments. What is the answer?
    
  ![image](https://github.com/user-attachments/assets/7aa1ff39-cd7e-4724-b12c-09fa2454eadd)

  Answer: 911cd574a42865a956ccde2d04495ebf

  I navigated to packet number 12 (Ctrl + G) and found a comment with this hash value. To view the full comment, I used the packet comment feature in the Edit menu.

![image](https://github.com/user-attachments/assets/22bf00c8-db9c-41e7-90a6-9bf31d4e8b16)

![image](https://github.com/user-attachments/assets/952f6c48-0a4b-4bb3-bb2f-e8b66d557342)

![image](https://github.com/user-attachments/assets/500ffb82-8369-46c8-b8c1-4f49dda080b5)

  ### There is a ".txt" file inside the capture file. What is the alien’s name?
  
  ![image](https://github.com/user-attachments/assets/49f7c6df-36a2-428b-8030-404c6620ebb2)

![image](https://github.com/user-attachments/assets/f757868e-f9cd-4895-826d-436e3584d6bc)

![image](https://github.com/user-attachments/assets/bce717fa-9cce-41e4-a803-1c4462a24131)

  Answer: PACKETMASTER

By exporting objects from the HTTP protocol (File > Export Objects), I found a .txt file within the capture. After saving and opening the file, I found that the alien’s name was PACKETMASTER.

### What is the number of warnings in the expert info section?

  ![image](https://github.com/user-attachments/assets/3b0949e8-b704-4198-a244-d71f2c59d190)

![image](https://github.com/user-attachments/assets/04b05734-ff88-464a-8485-10a2801bde46)

![image](https://github.com/user-attachments/assets/6a2768b0-8616-454f-a22a-907f971365d1)

![image](https://github.com/user-attachments/assets/b61b5c27-1d07-4d6f-88bb-4ce45c5c46c9)

![image](https://github.com/user-attachments/assets/cc3c3e0c-4c3a-4196-980f-e9ddd6e38fea)

  Answer: 1636

![image](https://github.com/user-attachments/assets/a65ebb7f-d638-41e5-b475-59ae67b0617c)

![image](https://github.com/user-attachments/assets/2c90eb3b-885d-41fb-981f-737859ca58ac)

  By accessing the Expert Information section (Analyze > Expert Information), I found the number of warnings listed at 1636.

### Task 5: Packet Filtering

  Go to packet number 4. Right-click on the “Hypertext Transfer Protocol” and apply it as a filter. What is the filter query?
  
  ![image](https://github.com/user-attachments/assets/b275c99d-44c2-4cbf-ba55-c1ae36075eae)

  Answer: http

  I navigated to packet number 4 (Ctrl + G), right-clicked on the HTTP protocol, and applied it as a filter. The applied filter query, http, was displayed in the filter pane.

### What is the number of displayed packets?

![image](https://github.com/user-attachments/assets/7ecc969a-01f7-476c-8eb3-4a8afd41f9bd)

  Answer: 1089

![image](https://github.com/user-attachments/assets/97d09a68-71e8-410b-9264-3951d5bca47f)

After applying the HTTP filter, the number of displayed packets was shown at the bottom right of the status bar, totaling 1089.

###  Go to packet number 33790 and follow the stream. What is the total number of artists?
        
  Answer: 3

I followed the HTTP stream for packet 33790 and searched for instances of the word “artist.” This led me to discover that there were three artists mentioned in the stream.

  ### What is the name of the second artist?

  ![image](https://github.com/user-attachments/assets/1b93319a-ba46-45d4-b6f5-0975cff2b48d)

![image](https://github.com/user-attachments/assets/386ca733-5e42-49e4-9d8d-083f1292f4ad)

![image](https://github.com/user-attachments/assets/5d5f4a06-7895-4d7f-b658-c8fcafd0701c)

  Answer: Blad3

![image](https://github.com/user-attachments/assets/182635f6-7c11-4b40-bcab-7d0b09099ee8)

By modifying the search query to "artist=2," I found that the name of the second artist was Blad3.

Conclusion:

This project helped me to develop a deeper understanding of network traffic analysis and how to extract specific information using Wireshark. I became familiar with navigating through packet captures, identifying key details within packet headers, and using search and filter functionalities to narrow down the data.
Experience Gained:

  Efficient navigation of packet captures using Wireshark’s filter and search functionalities.
  Understanding of protocol-level data (e.g., HTTP, TCP, IP) and how to extract relevant details from the OSI model layers.
  Practice with exporting objects and calculating hash values for files extracted from packet captures.

Benefits:

Enhanced ability to investigate network traffic in cybersecurity scenarios.
Improved skills in dissecting packets and understanding the significance of various protocol layers.
Knowledge of Wireshark’s powerful filtering and analysis features, enabling me to efficiently pinpoint crucial details during an investigation.


