[Back to Main Menu](https://github.com/CCC-Industry4/IIOT-4.0-Project/tree/main)

*Instruction to teacher: Divide into pairs. One person reads/researches each step, while the other performs the actions. Each pair will work independently with their own Smart Home setup.*
# Configure Smart Home
---
1. Connect the demonstration PC to the Pi. Wi-Fi can be used on a PC or smartphone. The disadvantages of using Wi-Fi are that you will lose access to the internet. Connect to the following:
SSID (service set identifier): IT4Project
Password: IOT12345
2. Plug in and powerup Smart Home.
3. Connect to the wifi address displayed on the Smart Home's LCD using a phone or laptop. 
	![LCD with URL](https://github.com/user-attachments/assets/2a204688-add5-4016-b089-6b25a3d443a6)
	![PXL_20260127_231858364](https://github.com/user-attachments/assets/44c8bdfe-92b0-4437-a84a-c9ed12e0df13)

	SSID (service set identifier): Config_ESP32
	Password: 012345678

5. Configure namespace of Smart Home using a web browser.
	While connected to Config_ESP32, navigate to the IP listed on the LCD screen using a web browser.
	![PXL_20260127_231935446](https://github.com/user-attachments/assets/be1445f4-0e8d-4762-bbfa-b91336e50bf9)

      ![Smart home Configuration page](https://github.com/user-attachments/assets/7aa42ee4-e932-437f-963c-6309f6642a7c)

  -  Ask your instructor for the neighborhood and home number:
      -  Neighborhood number- should be the same for the whole class.
      -  Home number- must be unique for each home in the neighborhood.
      -  Unless otherwise told, leave the other settings as their defaults.
        ![Finalize](https://github.com/user-attachments/assets/fa547931-8f3c-4cdc-b884-9069e87cc1b2)
	  - **Click Finalize and Reset ESP32.**

5. **Verify** that your Smart Home is working. 
  -  **Press CLOUD** then **LOCAL** buttons on the SCADA to cause the dropdown to include the new number.
  -  **Select** the new home number in the dropdown.
  -  If you see the count increasing simultaneously on the house and on the SCADA system on the web browser, you have successfully set-up the Arduino Smart Home.
6. You can not have two smart homes with the same namespace.  If your home doesn’t connect, look at the namespace of working SmartHome. 
7. Demonstrate to your instructor.
