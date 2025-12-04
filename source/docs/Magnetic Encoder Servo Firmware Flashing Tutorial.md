# Magnetic Encoder Servo Firmware Flashing Tutorial

> [!NOTE]
>
> **Taking HX-30HM as an example here,**

**Magnetic Encoder Servo** PC Software Installation Package path:  [Appendix/ServoStudio_0.1.1_x64-setup.exe](https://drive.google.com/drive/folders/1G2VSZiqwqcjcrp59oCFjL_C3VDzehWqo)

The wiring diagram for the servo control board is shown below. Power the board with a 12V power supply and connect the servo control board to the computer using a Type-C cable. Connect the magnetic encoder servo to the board.

<img src="..\_static\media\chapter_1\section_1\image_2.png" class="common_img" style="width:600px;"/>

Press **Win+R** to open the Control Panel, type **devmgmt.msc**, and open **Device Manager**.

<img src="..\_static\media\chapter_1\section_1\image_3.png" class="common_img" style="width:500px;"/>

Click **Ports** to view the port number; here, the port number is **COM10**.

<img src="..\_static\media\chapter_1\section_1\image_4.png" class="common_img" style="width:800px;"/>

Double-click to open the software <img src="..\_static\media\chapter_1\section_1\image_1.png" style="width:55px;"/>.

Follow the steps:  
Change the **Port** number to the one found (in this case, change to **COM10**\)   
-> Set the baud rate for **HX-30HM** to 1000000 

> [!NOTE]
>
> **The baud rate may vary for different magnetic encoder servos. Refer to the corresponding model's user manual for specifics.** 

-> Click **Connect**
-> Click **Scan**

<img src="..\_static\media\chapter_1\section_1\image_5.png" class="common_img" style="width:1200px;"/>

The system will scan all servo `ID`. If a servo is detected, a servo control interface will appear, as shown in the image below.

> [!NOTE]
>
> **If no servo is detected, unplug and re-plug the servo for testing.**

<img src="..\_static\media\chapter_1\section_1\image_6.png" class="common_img" style="width:1200px;"/>

Click **Firmware** -> Click **Click or drag firmware file here.**.

<img src="..\_static\media\chapter_1\section_1\image_7.png" class="common_img" style="width:1200px;"/>

Click the **HX-30HM_V3.9_20251023.sfw** firmware package -> Click **Open**.

<img src="..\_static\media\chapter_1\section_1\image_8.png" class="common_img" style="width:800px;"/>

Click **Force Upgrade** -> Click **Upgrade**.

<img src="..\_static\media\chapter_1\section_1\image_9.png" class="common_img" style="width:1200px;"/>

When the following screen appears, it indicates that the flashing process has started. At this point, unplug and re-plug the servo wire.

<img src="..\_static\media\chapter_1\section_1\image_12.png" class="common_img" style="width:1200px;"/>

When the red box appears, it indicates the servo firmware has been successfully flashed.

<img src="..\_static\media\chapter_1\section_1\image_11.png" class="common_img" style="width:1200px;"/>

> [!NOTE]
>
> **If a "Handshake Failed" message appears (as shown in the image below), follow the steps in the documentation to proceed again. Click "Upgrade" and retry the firmware flashing process.**

<img src="..\_static\media\chapter_1\section_1\image_10.png" class="common_img" style="width:1200px;"/>

