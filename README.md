
# NoMoreWatermark

## Description

NoMoreWatermark is a simple Python script that helps you remove the Windows watermark by using the "slmgr" command to reset the licensing status and then initiating a system restart to apply the changes.

## How to Use

1. Clone this repository to your local machine or download the script directly.

2. Open a terminal or command prompt.

3. Navigate to the directory where the script is located.

4. Run the following command:

   ```
   python remove_watermark.py
   ```

   Make sure you have Python installed on your system.

5. The script will execute the following commands:

   ```python
   import os
   os.system("slmgr /rearm")
   os.system("shutdown /r")
   ```

   - The "slmgr /rearm" command resets the licensing status, which can help remove the watermark.
   - The "shutdown /r" command restarts the system to apply the changes.

6. After the system restarts, check if the Windows watermark has been removed.

## Disclaimer

Use this script at your own risk. Modifying system settings can have unintended consequences, and it's essential to ensure you have appropriate permissions and backups in place.


