1. Solve Windows 11 Installer cannot choose edition 
   
   create a file called `ei.cfg`, put into `sources` folder in windows installer
   
   ```
   [EditionID]
   Professional
   [Channel]
   Retail
   ```

2. Skip windows 11 Network Setup:
   
   shift + F10  to open CMD
   
   `OOBE\BYPASSNRO`

3. Fix Windows 11 VM does not reduce size after deleting files
   
   - In the Windows 11 VM, open powershell or command prompt as admin.
   - Use these commands to remove bitlocker encryption:
     - Check the bitlocker encryption status:
       - `manage-bde -status`
     - Check the **Conversion Status** and **Percent Encrypted** values to verify that encryption is enabled
     - Disable bitlocker encryption:
       - `manage-bde -off C:`
     - Use the encryption status command above to check and verify when bitlocker encryption is down to 0%.
