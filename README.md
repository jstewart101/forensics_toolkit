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
* ### Autopsy
    * **Description:** This tool can be used to analyze images gathered previously by tools such as FTK. You can download the executable [here](https://www.sleuthkit.org/autopsy/download.php).
    * **Review:** I found this tool pretty easy to use, but the images are so large it took a long time to ingest them into Autopsy. Once the images were ingested though, this tool made it simple to navigate around them and search for things that may aid in the investigation. 
    * **How to use Autopsy:** 
         1. Download Autopsy from the link above
         2. Install Autopsy by running the .exe file
         3. Once Autopsy is running, select the image that you would like to ingest
            * Note: this may take hours to ingest. I preferred to leave it running overnight since it took so long. 
         4. After you've ingested the images you want to analyze, navigate around the file structure with the menu on the left-hand side of the application
            * If you want to analyze multiple images at once, you'll need to ingest them separately. 
         
         See [this link](http://www.sleuthkit.org/autopsy/docs/quick/) for more information on using Autopsy.

* ### Volatility
    * **Description:** This tool can be used to analyze memory dumps. You can download the executable [here](https://www.volatilityfoundation.org/26).
    * **Review:** I found this tool a little difficult to use as it doesn't have a GUI and I had to look up commands to run in it. Once I found some useful commands, I was able analyze the memory dump more efficiently.  
    * **How to use Volatility:** 
         1. Download Volatility from the link above
         2. Navigate to the folder where you installed the .exe file
         3. Execute volatility by entering the command below:
            * "E:\volatility_2.4.win.standalone\volatility-2.4.standalone.exe" imageinfo -f name_of_image.raw
               * Replace "name_of_image.raw" with the name of your memory dump you want to analyze. The command above will return information about the memory dump. 
         4. You can find a list of commands from their Github page at this [link](https://github.com/volatilityfoundation/volatility/wiki/Command-Reference).
         
         See [this link](https://www.howtoforge.com/tutorial/how-to-install-and-use-volatility-memory-forensic-tool/) for more information on using Volatility.

Malware Analysis
---
