# Bypass-Windows-10
Here the tutorial how to bypass login password windows 10 (This for educational purpose only, do not use this method to illegal activity)


### LIST REQUIREMENT ITEMS
1. Other Computer (to create bootable device)
2. USB Drive / Flashdisk (At least 8GB)
3. ISO Windows 10 Download from [Microsoft Official Website](https://www.microsoft.com/en-us/software-download/windows10) | [Archives.Org](https://archive.org/details/en-us_windows_10_consumer_editions_version_22h2_updated_feb_2023_x64_dvd_c29e4bb3)
4. [Rufus](https://rufus.ie/en/) for make bootable device

### TUTORIAL BEGIN
### 1. Start

  1. Download ISO Windows 10 [Microsoft Official Website](https://www.microsoft.com/en-us/software-download/windows10) | [Archives.Org](https://archive.org/details/en-us_windows_10_consumer_editions_version_22h2_updated_feb_2023_x64_dvd_c29e4bb3)
  2. Download [Rufus](https://rufus.ie/en/)

### 2. Create Bootable Device
  
  1. Plug USB to other computer
  2. Run Rufus
<img width="472" height="604" alt="3 (1)" src="https://github.com/user-attachments/assets/f6835e4b-b5fb-419f-b2a5-d1ee1d30b010" />

 
  3. Select disk ISO / Image and pick the ISO that we downloaded
  4. Don't forget in this STEP must carefully to choose Parition scheme

      >NOTES:
      >MBR IS LEGACY | GPT IS UEFI
      >
      >(PLEASE CHOOSE THE SCHEME LIKE YOUR COMPUTER THAT LOCKED, YOU COULD SEE IN BIOS > BOOT)

  5. Name volume whatever do you want
  6. Start and wait till bootable complete
     
### 3. Bypass Start


  1. Boot using Flash drive
  <img width="474" height="269" alt="Display CMD" src="https://github.com/user-attachments/assets/11fa51e7-7171-45e2-9ce5-a53db6efab75" />

  
  2. Click Shift + F10 to show up CMD display
  3. Check all your drive letter using command "diskpart" enter > "list volume" and note your label letter name "Windows"
  4. Type " Copy (Your windows letter, Example C:) C:\windows\system32\utilman.exe c:\windows\system32\utilman.exe.xxx"
   
     >THIS COMMAND TO COPY YOUR ORIGINAL UTILMAN
  
  5. Type "Copy C:\windows\system32\cmd.exe c:\windows\system32\utilman.exe"

     >THIS COMMAND TO REPLACE YOUR UTILMAN INTO CMD
  
  6. Restart computer and unplug your flash drive

### 4. Bypass Proceed

  1.  Click Ease of Access icon (bottom-right)

  <img width="600" height="427" alt="Untitled design (2)" src="https://github.com/user-attachments/assets/b1292ff9-1073-4ed2-a1e1-2a0127e2b983" />

     
  3.  A black Command Prompt window should appear — and it will be running as administrator
  4.  Type "Netplwiz" > enter

  <img width="472" height="604" alt="3 (1)" src="https://github.com/user-attachments/assets/5f55eac7-eb79-45fe-8648-035f0b24d021" />

     
  5.  App User Account appear > now click Reset Password

  <img width="463" height="513" alt="1" src="https://github.com/user-attachments/assets/eed56f94-7c1b-4b92-ba95-abe5a5a554a6" />




  6.  Input your new password & confirm password

  <img width="463" height="513" alt="2" src="https://github.com/user-attachments/assets/5417d5fa-645b-45d9-a378-d79fc2de0f54" />

  
  7.  Click OK
  8.  Click OK and now tried login with new password

     
### Done! You’ve Recovered Access 🎉


============================================================================================

## RESTORE UTILMAN 

  1. Run CMD as Administrator
  2. Type Copy C:\windows\system32\utilman.exe.bak C:\windows\system32\utilman.exe
  3. Restart the computer > and tried again ease of access


