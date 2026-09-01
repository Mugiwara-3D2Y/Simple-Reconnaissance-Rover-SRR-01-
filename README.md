# Simple-Reconnaissance-Rover-SRR-01-(3D-Model)

> **A project built for Hack Club.**
> *A flexible 4-wheel rover template built for exploration, monitoring, and field testing. Includes ready-to-print 3D models and editable CAD files so you can easily customize it for your own build.*
> **NOTE:** the only use of AI was for describing my project to create this README, about 25%

## Project Deliverables
*  **Onshape Document Link:** https://cad.onshape.com/documents/328f3c9bf33f08104aae075f/w/b1dc5a9cc62e4fa71f2e4275/e/ef0978b53d92c064744758d2?renderMode=0&uiState=6a70f9a548c682f8d7dcd9b6
*  **Print Ready Files:** Located at [/.stl files](./.stl%20files) and [/.step files](./.step%20files).

## Gallery
| Front View | Top View |
| :---: | :---: |
| <img width="1358" height="644" alt="SRR-01 Front View" src="https://github.com/user-attachments/assets/e14ba830-b85d-4f2e-864f-49843768059c" /> | <img width="1358" height="644" alt="SRR-01 Top View" src="https://github.com/user-attachments/assets/d172db4a-c65b-4154-b322-6cb03adde44f" /> |
| **Side View** | **Back View** |
| <img width="1358" height="644" alt="SRR-01 Side View" src="https://github.com/user-attachments/assets/9b89ff31-3c02-4136-90bf-e7e95da391d2" /> | <img width="1358" height="644" alt="SRR-01 Back View" src="https://github.com/user-attachments/assets/41cd10e3-5420-482c-9e92-550e2e3a1086" /> |

## Concept
This project is a flexible, modular base designed for building exploration and tracking rovers. Think of the chassis as an adaptable template, it’s built so you can easily mount whatever sensors your project requires, whether you're navigating open fields, detecting life forms, or tracking environmental stats like air quality and humidity. The interior layout is also completely open-ended, giving you plenty of room to set it up for either full autonomy or standard manual remote control.

## Motivation
Designing and building rovers is something I’ve done for a while now. After making several of them, I wanted to create a universal blueprint that saves time and is easy for anyone to build. The idea here is to give makers a reliable foundation that they can easily tweak, allowing them to specialize the rover for real-world applications like smart agriculture, environmental exploration, or recovery efforts.

## Tech Stack
*  **CAD Software:** Onshape
*  **Design Paradigm:** Parametric modeling
*  **Target Manufacturing Process:** FDM 3D Printing

## Features
* I designed this rover to be tough enough for the field but simple enough for anyone to actually build:
1. **Articulated Suspension Legs:**
   * To give the rover its wide stance and high ground clearance, the suspension arms utilize 3/4-inch PVC pipes as the structural bone template. The CAD-printed leg joints are designed to slide onto these pipes at a fixed angle, allowing the rover to climb over rocks, agricultural ridges, or debris without high-centering the main body.
2. **M3 Screw Fastener:**
   * Every single shell, joints, and mounting bracket is secured using standard M3 screws. By designing the entire chassis around a single fastener size, it simplifies assembly, keeps weight down, and ensures that anyone building this can easily source or swap out parts without needing a massive tool kit.
3. **Modular Sensor Mounts:**
   * The main body features built-in mounting points ready for hardware customizability. The top lid includes pre-modeled slots that can take various environmental sensors(like DHT22 or MQ135), while the angled front nose features a dedicated bracket for a camera and dual-port cutouts in-front and at the back for two ultrasonic sensors.
4. **Rugged Outboard Wheels & Fenders:**
   * The wheels are pushed far out to the corners of the frame to give the rover maximum stability on steep slopes. Each wheel includes an integrated fender to keep dirt and debris from kicking up into the moving joints during outdoor testing.
5. **Enclosed Electronics:**
   * The main body features a spacious, multi-faceted top lid labeled SRR-01. This protective shell fully encloses the internal compartment, keeping sensitive microcontrollers, motor drivers, and battery packs safe from dust, debris, or moisture during field operations.
  

## Production Settings
Since this project is designed as a template, the final slicing settings will ultimately depend on what material you choose and how tough you need your rover to be. That said, here are the recommended base settings I’ve used for printing a durable, field-ready build:

| Slicing Parameter | Recommended Setting |
| :--- | :--- |
| Material | PETG |
| Layer Height | 0.16 mm |
| Infill density | 20% |
| Infill Pattern | Gyroid |
| Perimeters | 4 |
| Top/Bottom Layers | 4 Top / 4 Bottom |
| Supports | Tree |

> **Tolerance Note:** The M3 screw holes and PVC pipe sockets in the CAD model are designed with standard clearance tolerances. If your printer tends to over-extrude slightly, set your slicer's **XY Size Compensation** to `-0.05 mm` or `-0.1 mm` so the PVC pipes slide snugly into the leg joints without needing forced reaming.

> Turn off "Don't create support under brigdes" for [Front Cover Chasis](./.stl%20files/Chasis/Chasis%20-%20Front%20Cover.stl) and [Back Cover Chasis](./.stl%20files/Chasis/Chasis%20-%20Back%20Cover.stl).

## Bill of Materials (BOM)

If you want to skip the CAD tweaking and jump straight into printing and assembling a fully functional rover, here is everything you need to build the base model (`SRR-01`):

### Hardware & Fasteners
* **3/4-inch PVC Pipe:** 2x 90mm and 6x 60mm (or cut to your desired length for the leg joints).
* **M3 Screw Pack:** 
  * M3 × 8mm, 12mm and 40mm Screws 
  * M3 Hex Nuts 
* **Wheels:** 4x 65mm Robot Smart Car Wheels (Hex hub compatible for couplers)
* **Couplers:** 4x 18mm Hex couplings

### Recommended Core Electronics
* **Microcontroller** ESP32 or Arduino Uno
* **Motors:** 4x JGA25-370
* **Motor Drivers:** 2x L298N
* **Power Source:** 2S/3S LiPo battery pack or a 6×AA battery holder
* **GPS:** Ublox Neo GPS Module

### Sensors
* **Camera:** Logitech c270 web cam (or any other camera)
* **2x HC-SR04 Ultrasonic Sensors** 
* **DHT11 / DHT22 Temperature & Humidity sensor**
* **MQ-135 Gas sensor**

## Printing Process

Below outlines the time it takes to print each part based on the Production Settings.

| Part | Time |
| :--- | :--- |
| [Front Base Chasis](./.stl%20files/Chasis/Chasis%20-%20Front%20Base.stl) | **6 hours** |
| [Back Base Chasis](./.stl%20files/Chasis/Chasis%20-%20Back%20Base.stl) | **7 hours** |
| [Front Cover Chasis](./.stl%20files/Chasis/Chasis%20-%20Front%20Cover.stl) | **9 hours 30 minutes** |
| [Back Cover Chasis](./.stl%20files/Chasis/Chasis%20-%20Back%20Cover.stl) | **11 hours 30 minutes** |
| [Left Hand Chasis](./.stl%20files/Chasis/Chasis%20-%20Left%20Hand.stl) | **2 hours 20 minutes** |
| [Right Hand Chasis](./.stl%20files/Chasis/Chasis%20-%20Right%20Hand.stl) | **2 hours 20 minutes** |
| [Right Front PVC Pipe Joint](./.stl%20files/PVC%20Pipe%20Joint/PVC%20Pipe%20Joint%20-%20(Right%20Front%20or%20Left%20Rear).stl) | **1 hours 40 minutes** |
| [Right Rear PVC Pipe Joint](./.stl%20files/PVC%20Pipe%20Joint/PVC%20Pipe%20Joint%20-%20(Right%20Rear%20or%20Left%20Front).stl) | **1 hours 40 minutes** |
| [Left Rear PVC Pipe Joint](./.stl%20files/PVC%20Pipe%20Joint/PVC%20Pipe%20Joint%20-%20(Right%20Front%20or%20Left%20Rear).stl) | **1 hours 40 minutes** |
| [Left Front PVC Pipe Joint](./.stl%20files/PVC%20Pipe%20Joint/PVC%20Pipe%20Joint%20-%20(Right%20Rear%20or%20Left%20Front).stl) | **1 hours 40 minutes** |
| [Left Front Wheel Mount](./.stl%20files/Wheel%20Mount/Wheel%20Mount%20-%20Left%20Front.stl) | **3 hours 30 minutes** |
| [Left Rear Wheel Mount](./.stl%20files/Wheel%20Mount/Wheel%20Mount%20-%20Left%20Rear.stl) | **3 hours 20 minutes** |
| [Right Front Wheel Mount](./.stl%20files/Wheel%20Mount/Wheel%20Mount%20-%20Right%20Front.stl) | **3 hours 30 minutes** |
| [Right Rear Wheel Mount](./.stl%20files/Wheel%20Mount/Wheel%20Mount%20-%20Rigth%20Rear.stl) | **3 hours 20 minutes** |
| **Total** | **59 hours** |

## Assembly Guide

Assembling the base `SRR-01` takes about 30–45 minutes once all your parts are printed. Here is how it goes together:

### Step 1: eLower Chasis
* **Get the [Front Base](./.stl%20files/Chasis/Chasis%20-%20Front%20Base.stl) and [Back Base](./.stl%20files/Chasis/Chasis%20-%20Back%20Base.stl) of the chasis and insert an HC-SR04 ultrasonic sensor in each part.**
<table>
  <tr>
    <td align="center">
      <img width="1910" height="915" alt="STEP 1" src="https://github.com/user-attachments/assets/aeca6c52-1c82-4fc7-bd4f-fb9021d0d161" />
    </td>
    <td align="center">
      <img width="1910" height="915" alt="STEP 3" src="https://github.com/user-attachments/assets/80d4b5d3-2c30-4799-a861-3182dcd49ee6" />
    </td>
  </tr>
  <tr>
    <td align="center">
      <img width="1910" height="915" alt="STEP 2" src="https://github.com/user-attachments/assets/c354ae0d-8f27-4e94-8c80-3e48cb272127" />
    </td>
    <td align="center">
      <img width="1910" height="915" alt="STEP 4" src="https://github.com/user-attachments/assets/e9ad39c5-b7b2-4834-9362-67fee4f5eac1" />
    </td>
  </tr>
</table>

* **Join the two bases together then fasten them with 3 m3*8mm Screws and nuts**
<table>
  <tr>
    <td align="center">
      <img width="1910" height="915" alt="STEP 6" src="https://github.com/user-attachments/assets/7cf2b877-2d5a-4a28-a88d-f75fb0a0ceda" />
    </td>
    <td align="center">
      <img width="1910" height="915" alt="STEP 7" src="https://github.com/user-attachments/assets/0d5078c5-c832-44ae-b42b-e6eb7b878fd1" />
    </td>
  </tr>
</table>

* **Add the [Left Hand](./.stl%20files/Chasis/Chasis%20-%20Left%20hand.stl) and [Right Hand](./.stl%20files/Chasis/Chasis%20-%20Right%20hand.stl) to the base respectively. After that fasten them with 8 m3*8mm Screws and nuts**
<table>
  <tr>
    <td align="center">
      <img width="1669" height="945" alt="STEP 9" src="https://github.com/user-attachments/assets/f7e5813f-b2e2-4350-9407-97f85012aeb7" />
    </td>
    <td align="center">
      <img width="1669" height="945" alt="STEP 10" src="https://github.com/user-attachments/assets/458af059-8f7c-416d-be9c-f5c2a251a6f7" />
    </td>
  </tr>
</table>

### Step 2: Rover Legs
* **Slide a JGA25-370 motor into the [Left Front Wheel Mount](./.stl%20files/Wheel%20Mount/Wheel%20Mount%20-%20Left%20Front.stl) with two m3*12mm Screws.**
<table>
  <tr>
    <td align="center">
      <img width="1910" height="915" alt="STEP 11" src="https://github.com/user-attachments/assets/5d9940b2-1f24-4d63-b80c-6b346dd6fbef" />
    </td>
    <td>
      <img width="1910" height="915" alt="STEP 12" src="https://github.com/user-attachments/assets/c1fcccf9-a79b-434e-9c7b-5c27ec018af1" />
    </td>
    <td>
      <img width="1910" height="915" alt="STEP 13" src="https://github.com/user-attachments/assets/582c7a1b-a54d-4ec8-b533-1cd7bb92f02f" />
    </td>
  </tr>
</table>

* **Next fix one 30mm PVC Pipe in the [Left Front Wheel Mount](./.stl%20files/Wheel%20Mount/Wheel%20Mount%20-%20Left%20Front.stl) followed by the [Left Front PVC Pipe Joint](./.stl%20files/PVC%20Pipe%20Joint/PVC%20Pipe%20Joint%20-%20(Right%20Rear%20or%20Left%20Front).stl) aligned correspondingly.**
<table>
  <tr>
    <td align="center">
      <img width="1910" height="915" alt="STEP 14" src="https://github.com/user-attachments/assets/2ada1372-04d7-4e9c-bdd1-825ff98327e2" />
    </td>
    <td align="center">
      <img width="1910" height="915" alt="STEP 15" src="https://github.com/user-attachments/assets/15d1e8d7-7ca9-4cb0-a347-047993ed475f" />
    </td>
  </tr>
</table>

* **After that, fit a 60mm Pipe into the [Left Front PVC Pipe Joint](./.stl%20files/PVC%20Pipe%20Joint/PVC%20Pipe%20Joint%20-%20(Right%20Rear%20or%20Left%20Front).stl)**
<table>
  <tr>
    <td align="center">
      <img width="1910" height="915" alt="STEP 16" src="https://github.com/user-attachments/assets/17505e66-51fd-4728-a890-027976c504b8" />
    </td>
    <td align="center">
      <img width="1910" height="915" alt="STEP 17" src="https://github.com/user-attachments/assets/1e7c626b-ce1a-4ccc-823e-7a9f058df286" />
    </td>
  </tr>
</table>

* **Repeat Steps 2.1, 2.2 and 2.33 with the [Left Rear Wheel Mount](./.stl%20files/Wheel%20Mount/Wheel%20Mount%20-%20Left%20Rear.stl), [Left Rear PVC Pipe Joint](./.stl%20files/PVC%20Pipe%20Joint/PVC%20Pipe%20Joint%20-%20(Right%20Front%20or%20Left%20Rear).stl) and a 30mm PVC Pipe**
<table>
  <tr>
    <td align="center">
      <img width="1910" height="915" alt="STEP 18" src="https://github.com/user-attachments/assets/e5b4afb6-ae11-4ac6-8d66-9c49124b036f" />
    </td>
    <td align="center">
      <img width="1910" height="915" alt="STEP 19" src="https://github.com/user-attachments/assets/e535af46-8abb-458e-9d2c-0af247153833" />
    </td>
  </tr>
  <tr>
    <td align="center'>
      <img width="1910" height="915" alt="STEP 20" src="https://github.com/user-attachments/assets/ab3b5655-7d14-4e17-8904-0946664b2134" />
    </td>
    <td align="center">
     <img width="1910" height="915" alt="STEP 21" src="https://github.com/user-attachments/assets/e4b88bf9-f010-4eb8-ac80-c9720bcdaee3" />
    </td>
  </tr>
  <tr>
    <td align="center">
      <img width="1910" height="915" alt="STEP 22" src="https://github.com/user-attachments/assets/344667ec-8f06-45a4-9693-b26749a6a265" />
    </td>
    <td align="center">
      <img width="1910" height="915" alt="STEP 23" src="https://github.com/user-attachments/assets/35845add-6232-47c1-bb4b-296ef82b84d3" />
    </td>
  </tr>
</table>

* **Gather the two separate assemblies and add them to the Bottom Chasis from Step 1.**
<table>
  <tr>
    <td align="center">
      <img width="1910" height="915" alt="STEP 24" src="https://github.com/user-attachments/assets/c9fd454d-b7a9-4ec3-ae01-9c06fc491f42" />
    </td>
    <td align="center">
      <img width="1910" height="915" alt="STEP 25" src="https://github.com/user-attachments/assets/0afbf175-4d93-4105-8e11-498ada35ea82" />
    </td>
  </tr>
</table>

* **Repeat the whole of Step 2 so far with [Right Front Wheel Mount](./.stl%20files/Wheel%20Mount/Wheel%20Mount%20-%20Right%20Front.stl), [Right Rear Wheel Mount](./.stl%20files/Wheel%20Mount/Wheel%20Mount%20-%20Rigth%20Rear.stl), [Right Front PVC Pipe Joint](./.stl%20files/PVC%20Pipe%20Joint/PVC%20Pipe%20Joint%20-%20(Right%20Front%20or%20Left%20Rear).stl) and [Right Rear PVC Pipe Joint](./.stl%20files/PVC%20Pipe%20Joint/PVC%20Pipe%20Joint%20-%20(Right%20Rear%20or%20Left%20Front).stl).**
<table>
  <tr>
    <td align="center">
      <img width="1910" height="915" alt="STEP 26" src="https://github.com/user-attachments/assets/818b0f86-668f-4b6a-a1ec-5d7ca9fe3ad3" />
    </td>
    <td align="center">
      <img width="1912" height="948" alt="STEP 27" src="https://github.com/user-attachments/assets/577b2ac3-e48c-4a02-811b-a3fb1e35c04b" />
    </td>
  </tr>
</table>

### Step 3: Upper Chasis
* **Attach a DHT22 Temperature & Humidity sensor, an Ublox Neo GPS and a MQ-135 Gas sensor to the [Back Cover Chasis](./.stl%20files/Chasis/Chasis%20-%20Back%20Cover.stl). Use 4 m3*5mm Screws to fasten the Gas sensor.
<table>
  <tr>
    <td align="center">
      <img width="1912" height="948" alt="STEP 29" src="https://github.com/user-attachments/assets/5cde2310-76ae-4d40-ac2f-0bbc4c535cfe" />
    </td>
    <td align="center">
      <img width="1912" height="948" alt="STEP 30" src="https://github.com/user-attachments/assets/507234b0-ad74-4184-a7c4-c48e99b89882" />
    </td>
    <td align="center">
      <img width="1912" height="948" alt="STEP 31" src="https://github.com/user-attachments/assets/870e122c-a6b5-4896-9c4e-10bc2f33b3c8" />
    </td>
  </tr>
</table>

* **Now fasten the [Back Cover Chasis](./.stl%20files/Chasis/Chasis%20-%20Back%20Cover.stl) to the Bottom Chasis with 2 m3*40mm**
<table>
  <tr>
    <td align="center">
      <img width="1912" height="948" alt="STEP 32" src="https://github.com/user-attachments/assets/fd5f0761-7404-41b6-a94a-07696fc7a39b" />
    </td>
    <td align="center">
      <img width="1912" height="948" alt="STEP 33" src="https://github.com/user-attachments/assets/360e5ae7-a294-4e91-9080-71d21e7c6999" />
    </td>
  </tr>
</table>

* **Take the [Front Cover Chasis](./.stl%20files/Chasis/Chasis%20-%20Front%20Cover.stl) and attach a camera to the space infront.**
<table>
  <tr>
    <td align="center">
      <img width="1912" height="948" alt="STEP 34" src="https://github.com/user-attachments/assets/671c59c1-2001-433b-ad7f-f5786c5387ad" />
    </td>
    <td align="center">
      <img width="1912" height="948" alt="STEP 35" src="https://github.com/user-attachments/assets/6ec5ad61-e128-4c72-9d42-b6b3762d030d" />
    </td>
  </tr>
</table>

* **Fix the [Front Cover Chasis](./.stl%20files/Chasis/Chasis%20-%20Front%20Cover.stl) to the Bottom Chasis with 2 m3*40mm and 2 m3*

>  Working on it...
