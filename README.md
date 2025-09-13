## Install Autopsy and Analyze the Disk File and Folder Configuration

## AIM
To install **Autopsy** and use it to analyze the disk’s file and folder configuration for forensic investigation.

## REQUIREMENTS
- **Operating System**: Windows 10/11, macOS, or Linux
- **Tools**:  
  - [Autopsy Digital Forensics Platform](https://www.autopsy.com/)  
  - Optional: Sleuth Kit CLI tools for deeper analysis
- **Test Data**: Disk image file (`.dd`, `.img`, `.E01`)

## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Install Autopsy]
    B --> C[Create New Case in Autopsy]
    C --> D[Add Data Source: Disk Image]
    D --> E["Autopsy Modules Run: File System, Metadata, Keywords"]
    E --> F[File & Folder Structure View]
    F --> G[Export / Recover Files]
```
## DESIGN STEPS:
### Step 1:
Download Autopsy from the official website and install it on your system.

### Step 2:
Launch Autopsy and create a new case.

### Step 3:
Add your disk image or physical drive as the data source.

### Step 4:
Allow Autopsy to run its built-in ingest modules (file system analysis, hash lookup, keyword search, metadata extraction).

### Step 5:
View the file and folder hierarchy in the left-hand tree panel.

### Step 6:
Export or recover files if required for the investigation.

## PROGRAM(Windows)

1. Download Autopsy from autopsy.com.
2. Install and launch the application.
3. Select **New Case → Name your case → Choose case folder**.
4. Click Add **Data Source → Select Disk Image → Browse to file**.
5. Choose ingest modules (file system, metadata, hash lookup, keyword search).
6. Wait for processing to finish.
7. Explore file/folder structure in the navigation pane.
8.Export selected files for further examination.

## CREATING A DISK PARTITION:
Step1: Open File Manager
● Right-click This PC → Click Show More Options.

● Select Manage.

Step2: Access Disk Management
● In the new window, select Disk Management.

Step3: Shrink the C Drive to Allocate Space
• Locate C: drive → Right-click → Select Shrink Volume.
• Enter the amount of memory to allocate for the new disk.
• Click Shrink.

Step4: Create a New Volume
• Right-click on the newly unallocated space → Select New Simple Volume.

• Follow the wizard and assign a disk name.

• Click Finish to complete the process.

• The new Disk Partition is created
## ANALYSING FILES USING AUTOPSY:
Step1: Create a Case
• Enter a case name and select a location to store the case data.

• Provide a case number and investigator details if required.

Step2: Add a Data Source
• Click "Add Data Source" and choose the type:

• Select the data source and let Autopsy process it.
Step3: File Analysis
• Application

<img width="1919" height="1079" alt="Screenshot 2025-09-13 212654" src="https://github.com/user-attachments/assets/f0240ceb-04ad-4401-a969-ef7986c18acb" />

<img width="1915" height="1077" alt="Screenshot 2025-09-13 212644" src="https://github.com/user-attachments/assets/b4f11aa7-0bed-4519-98c1-8f920599315e" />


<img width="1919" height="1079" alt="Screenshot 2025-09-13 212457" src="https://github.com/user-attachments/assets/f3f75695-59af-4ca0-9c00-b7f1b7db6826" />


• File Metadata
<img width="1918" height="1079" alt="Screenshot 2025-09-13 212525" src="https://github.com/user-attachments/assets/fa8daab3-9824-4fbc-b8d7-939aa213609e" />



## OUTPUT:
Report

<img width="1919" height="1079" alt="Screenshot 2025-09-13 212627" src="https://github.com/user-attachments/assets/72fd449d-f351-47cf-9063-0fc7a1816fd4" />


## RESULT:
Autopsy was installed successfully and used to analyze disk, file, and folder configuration for forensic investigation.
