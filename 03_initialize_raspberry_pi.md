[Back to Main Menu](https://github.com/CCC-Industry4/IIOT-4.0-Project/tree/main)
# Initialize Raspberry Pi
# Cloning github repository on the Pi
1. Begin by cloning this repo in your Linux terminal: git clone https:https://github.com/CCC-Industry4/IIOT-4.0-Project
2. After it finishes cloning, enter the directory using: cd IIOT-4.0-Project
3. Run the some_installs.sh script to download dependencies: ./some_installs.sh
After these steps, all the dependencies for Mosquitto and dearImgui are downloaded. Now you can begin working on building the rest of the project.

# Downloading Ignition Gateway on the Pi
You can run the Ignition Gateway on a Raspberry Pi and use Ignition Designer. Download the Gateway on the Pi and PC. Then run the Designer on your PC to view the project we have. See the [Ignition Quick Start Guide](https://docs.inductiveautomation.com/display/DOC80/Quick+Start+Guide). The steps are as follows:
1. Download Ignition [here](https://inductiveautomation.com/downloads/ignition/8.1.31) and be sure to chose the correct one for your Operating System. If you run a Raspberry Pi OS on a 64 bit Architecture, you should choose Ignition - Linux AARCH64 zip.
2. After your Download finishes, open your terminal and enter the Downloads folder using cd Downloads.
3. Next, run the following command to unzip the downloaded folder: sudo unzip {name of Downloaded file} -d /usr/local/ignition
4. After the folder finishes unzipping, enter the new directory: cd /usr/local/ignition/
5. Next, run this command to make all necessary files executable: sudo chmod +x *.sh ignition-gateway
6. Then run the now executable Ignition script: sudo ./ignition.sh start. Congratulations! The Ignition Gateway has started.
7. Now, enter your browser and run the local host: localhost:8088. Give the Gateway a few minutes to start.
8. The first time you open it, it will ask you which form of Ignition you want to use. Choose the one that best fits your needs, but we chose Full Ignition when building this project.
9. Now Ignition is running on the Raspberry Pi!
Now that Ignition is downloaded, you can start ignition any time from the terminal by entering cd /usr/local/ignition then running the script sudo ./ignition.sh start. Then open the gateway by entering in your browser localhost:8088 and you will be able to view the gateway!

# Installing MQTT Modules on Ignition
To install the MQTT modules for Ignition, you must do the following (see this video for more information): [Video Link](https://youtu.be/AB4knX_4n5c)
1. Use this [link](https://inductiveautomation.com/downloads/third-party-modules/8.3.3) and locate the MQTT Distributor, Transmission, and Engine modules. Download all three and then from your Ignition Gateway you should be able to install the modules using the *.modl files you downloaded.
2. Open the MQTT server using the web browser on the Pi.In a web browser, type http://localhost:8088 to the ignition server.
3. Go to Config/Sytem/Modules then locate "Install or Upgrade a Module..." at the bottom of the page.
4. Now you will see these modules listed at the bottom of the Config bar.

# Configuring MQTT Engine Module on Ignition
1. Click on Config/MQTT Engine/Settings.
2. In the General Tab unselect: "Block outbound edge node tag writes" and "Block outbound device tag writes." Then save changes.
3. Under Servers "Create new MQTT Server Settings. Name new Server "PI" (so that this matches other files you download). Add URL (i.e. tcp://192.168.10.2.) Then click "Create New MQTT Server Settings."
4. Under Namespace/Custom give a name and put the # sound to subscribe to everything, then save changes.

# Ignition Licenses for Education
Ignition allows individuals to use full ignition on a two hour resettable trial basis indefinitely for non commercial use.  Alternatively Ignition Maker Edition, a streamed down version, may be used for personal use without the need for resetting, but must be connected to the internet.   Inductive Automation partners with qualifying educational institutions to provide free Ignition licenses to students anywhere in the world! Apply here: [https://inductiveautomation.com/educational-engagement](https://inductiveautomation.com/educational-engagement)

# Object Detection using YOLOv5
1. To install YOLOv5 in the repository run ./ObjectDetection/install.sh
2. To run it use ./ObjectDetection/start.sh 

# Training YOLOv5
Clone the (labelImg repository)[https://github.com/HumanSignal/labelImg](https://github.com/HumanSignal/labelImg) and the YOLOv5
