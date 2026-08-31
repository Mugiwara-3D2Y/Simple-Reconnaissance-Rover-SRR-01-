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
| [Front Base](./.stl%20files/Chasis/Chasis%20-%20Front%20Base.stl) and [Back Base](./.stl%20files/Chasis/Chasis%20-%20Back%20Base.stl) | **6 hours** |
| [Back Base](./.stl%20files/Chasis/Chasis%20-%20Back%20Base.stl) | **7 hours** |
| [Front Cover](./.stl%20files/Chasis/Chasis%20-%20Front%20Cover.stl) | **9 hours 30 minutes** |
| [Back Cover](./.stl%20files/Chasis/Chasis%20-%20Back%20Cover.stl) | **11 hours 30 minutes** |
| [Left Hand](./.stl%20files/Chasis/Chasis%20-%20Left%20Hand.stl) | **2 hours 20 minutes** |
| [Right Hand](./.stl%20files/Chasis/Chasis%20-%20Right%20Hand.stl) | **2 hours 20 minutes** |
| [PVC Pipe Joint - (Right Front or Left Rear)](./.stl%20files/PVC%20Pipe%20Joint/PVC%20Pipe%20Joint%20-%20(Right%20Front%20or%20Left%20Rear).stl) | **1 hours 40 minutes** |

## Assembly Guide

Assembling the base `SRR-01` takes about 30–45 minutes once all your parts are printed. Here is how it goes together:

### Step 1: Chasis
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

  
>  Working on it...
