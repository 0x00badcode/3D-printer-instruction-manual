# 3D printer instruction manual


```diff
-⚠️ DO NOT USE ABS,USE ONLY PLA ⚠️   
-ABS IS TOXIC WHEN USED IN OPEN PRINTERS, DO NOT USE
````

legacy user manual : [https://c-3d.niceshops.com/upload/file/swx2-20210831_Manual.pdf](https://c-3d.niceshops.com/upload/file/swx2-20210831_Manual.pdf)


## Table of Contents

- [**Turning The Printer On**](#turning-the-printer-on)
- [**Turning It Off**](#turning-it-off)
- [**Changing the Filament**](#changing-the-filament)
  - [**Getting the Old Filament Out**](#getting-the-old-filament-out)
  - [**Putting the New Filament In**](#putting-the-new-filament-in)
- [**Preparing a File for Printing**](#preparing-a-file-for-printing)
- [**Print**](#print)
- [**Stopping a Print**](#stopping-a-print)
- [**Removing an Object from the Magnetic Bed**](#removing-an-object-from-the-magnetic-bed)
- [**Dealing with Print Issues**](#dealing-with-print-issues)


# **Turning The Printer On** {#turning-the-printer-on}

1. Locate the red power button at the back of the printer, next to the power cable.    

2. Switch the red power button to turn on the printer.

3. Wait for the printer to boot up. You will know it has completed the booting process when the screen lights up and the menu appears.

4. Once the screen is lit up and the menu is visible, the printer is ready to be used.

It's as easy as that! Now you can proceed with the desired actions on the Artillery X2.

# **Turning It Off** {#turning-it-off}

1. Ensure that any ongoing prints have completed or been canceled before turning off the printer.
 
2. Locate the red power button at the back of the printer, next to the power cable.

3. Press and hold the red power button for a few seconds until the screen turns off and the printer shuts down.

4. Once the printer has completely powered off, you can safely unplug it from the power outlet.

Remember to always power off the printer properly to prevent any potential damage or data loss.

# **Changing the Filament**

To ensure a smooth filament change process, follow these steps:

## **Getting the Old Filament Out:**

1. Cut the filament just above the printer's head to minimize filament loss.

2. Navigate to the printer's base menu.

3. Click on **Tools** and select **Change** from the options.

4. Gently pull the filament that protrudes from the printer. If it comes out easily, great! If not, avoid excessive force.

5. Click on **Out** to extrude the remaining filament. As the filament is extruded, use tweezers to remove it from the path and prevent it from clogging the printer's head. 
(Tweezers can be found in the hub; search around to locate them.)

6. Once all the filament is successfully removed, the printer will notify you to proceed to the next step: loading the new filament.

7. If you encounter any issues, feel free to seek assistance from Paul Crinquand or Erwan Molina on campus. They will be happy to help you with the printer setup.

## **Putting the New Filament In:**

Before proceeding with the following steps, ensure that the "Getting the Old Filament Out" process has been completed.

1. Take a new **PLA** filament and place it on the filament support located on top of the printer.

2. Pull the little black lever and insert the filament into the hole at the top of the printer.

3. While continuing to hold the lever, feed the filament into the printer's head until it cannot be inserted further.

4. Click on **In** and wait for the printer to pull the filament in.

5. As in the previous step, you will need to handle some excess filament; however, there will be more of it this time.

6. Once the printer notifies you that the new filament is loaded, you are ready to start printing.

7. If you encounter any problems, don't hesitate to reach out to Paul Crinquand or Erwan Molina on campus for assistance with the printer setup. They will be glad to help you.

Note: Proper filament handling and setup are crucial for successful printing.

## **Preparing a File for Printing**

To prepare a file for printing on the Artillery X2, follow these steps:

1. Choose a slicer software of your preference. In this example, we will use Cura slicer, which can be downloaded from **[https://ultimaker.com/software/ultimaker-cura/](https://ultimaker.com/software/ultimaker-cura/)**.

2. Install Cura on your computer and launch the software.

3. Click on "Add Printer" in Cura and select "Non-Networked Printer." Choose "Artillery" and then select "Artillery SideWinger X1."

4. Scroll down to the "Start G-Code" box at the bottom of the page. Copy and paste the provided G-Code into this box, and then click "Next."

```jsx
G28 ; home all axes
G29 ; Bed autolevel
M117 Purge extruder
G92 E0 ; reset extruder
G1 Z1.0 F3000 ; move z up little to prevent scratching of surface
G1 X2 Y20 Z0.3 F5000.0 ; move to start-line position
G1 X2 Y200.0 Z0.3 F1500.0 E15 ; draw 1st line
G1 X2 Y200.0 Z0.4 F5000.0 ; move to side a little
G1 X2 Y20 Z0.4 F1500.0 E30 ; draw 2nd line
G92 E0 ; reset extruder
G1 Z1.0 F3000 ; move z up little to prevent scratching of surface
```

5. Go to "File" and select "Open File" to load a 3D file for printing. The supported file formats include STL, OBJ, X3D, 3MF, as well as image formats like BMP, GIF, JPG, and PNG.

6. Once the file is loaded, it will appear in the editor. Use the sidebar options to resize, rotate, and position the object on the printing bed. The editor will indicate if the object is out of bounds.

7. After positioning the object, access the settings in the top right corner. Configure the infill density (the degree of filling in the piece; lower values result in faster but less sturdy prints, while 20% is suitable for regular pieces), and enable supports if necessary. For further customization, click on "Custom."

8. Click on "Slice" to process the model. The software will provide information about the estimated printing time and filament usage. If you are satisfied with the settings, click "Save to Disk" and save the file in .gcode format. You can save it to your USB drive or use the mounted USB drive on the printer itself.

# **Print**

1. On the printer's screen, select the option labeled "Print."

2. Use the right and left arrows on the screen to navigate through the available files.

3. Choose the desired file by selecting it, and then click on **Confirm** to proceed.

4. The printing bed and the printer's head will begin to heat up. It is crucial to note that during this process, you should avoid touching either the bed or the head. ⚠️ Do not touch ⚠️.

5. After a short period, the printer will initiate movement and calibration. It is essential to refrain from blocking the printer's movement, touching it, or placing any objects on it.

# **Stopping a Print**

1. On the printer's screen, locate and select the "Options" button.

2. In the options menu, choose the "Stop" option to halt the ongoing print.

3. Allow the printer to complete its current movements and retract the extruder. Avoid touching or interfering with the printer during this process.

4. Once the printer has finished its movements and is in a safe position, you can carefully remove your print from the print bed.

# **Removing an Object from the Magnetic Bed**

1. Ensure that the printer has completed the print and is turned off or in a paused state.

2. Locate the handle in the middle of one of the corners of the magnetic bed.

3. Firmly grasp the handle and gently lift the magnetic bed away from the printer's build plate.

4. Take caution not to scrape or damage the bed while handling it.

5. Once the magnetic bed is removed, carefully bend it to flex and release the printed object.

6. Slowly and steadily peel back the magnetic bed to separate it from the printed piece, being careful not to apply excessive force or use sharp objects that could damage the bed.

7. After the object is successfully removed, place the magnetic bed back onto the printer's build plate, ensuring proper alignment and attachment.

# **Dealing with Print Issues**

In the event of a print failure or error on the Artillery X2, follow these steps to address the situation:

1. Power off the printer to stop any further printing actions or movements.

2. Gently move the printer arms out of the way to create space for troubleshooting.

3. Refer to the "Removing an Object from the Magnetic Bed" section mentioned earlier to safely remove any partially printed or failed object from the magnetic bed.
    - Follow the steps outlined in that section, beginning with grasping the handle in the middle of one of the corners of the magnetic bed.
    - Exercise caution while bending the bed to release the failed print, ensuring not to scrape or damage the bed during the removal process.
