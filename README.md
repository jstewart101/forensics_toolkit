# Forensics Toolkit
This respository was created for the Digital Forensics class taught at Brigham Young University. It contains forensics tools and resources that can be used during a digital forensics investigation. 

Forensic Imaging
---
* ### FTK Imager
    * **Description:** This tool can be used to gather images from machines involved in the investigation. It is made by Access Data and is a Windows based software. You can download the executable [here](https://accessdata.com/product-download/ftk-imager-version-4.2.0).
    * **Review:** I found this tool fairly easy to use and there is a lot of documention on it. I would highly recommend it if you need to take an image of a computer. It can be used to take a full image or just a memory dump. 
    * **How to use FTK Imager:** 
         1. Download FTK from the link above
         2. Install FTK and run FTKImager.exe
         3. Click on "File" in menu
         4. Select "Create a Disk Image", then choose the source of the image
         5. Add an "Image Destination"
         
         See [this link](https://digital-forensics.sans.org/blog/2009/06/18/forensics-101-acquiring-an-image-with-ftk-imager/) for more information on acquiring disk images. 
         
Network Analysis
---
* ### Wireshark
    * **Description:** This tool can be used to capture or analyze packet capture files. This will assist during an investigation to determine what kinds of traffic are going in and out of your network. You can download the executable [here](https://www.wireshark.org/download.html).
    * **Review:** I found this tool extremely easy to use and very intuitive. There are a lot of things to learn with Wireshark, but with having a basic understanding of networks, most analysts should find this tool easy to use. 
    * **How to use Wireshark:** 
         1. Download Wireshark from the link above
         2. Install Wireshark by running the .exe file
         3. Once Wireshark is running, select the connection you'd like to capture network traffic on
         4. After you've clicked on the connection it should start capturing packets on that interface
            * If you need to restart the capture, press the red "Stop" button and then the shark fin to "Start" 
         
         See [this link](https://www.wireshark.org/docs/) for more information on using Wireshark. 
Memory Analysis
---

Malware Analysis
---
