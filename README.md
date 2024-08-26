# save-me-from-my-mac

A collections of utility scripts or commands I write and gather to enhance macos experience

1. Adjust MacOS menubar padding 
   `defaults -currentHost write -globalDomain NSStatusItemSelectionPadding -int 8`

2. Time Machine Speed Up
   `sudo sysctl debug.lowpri_throttle_enabled=0`

3. Delete Local Snapshots (when deleting files does not release space)
   `for d in $(tmutil listlocalsnapshotdates | grep "-"); do sudo tmutil deletelocalsnapshots $d; done`

4. Network Quality
   `networkquality`

5. SSD WR Info
   `sudo smartctl --all /dev/disk0`

6. Add executing permission 
   `chmod +x xxx.sh`

7. Full CPU One Core Load
   `yes > /dev/null`

8. Remove Quarantine
   `sudo xattr -d com.apple.quarantine xxx.app`

9. Keep MacOS Awake
   `caffeinate`

10. Calc MD5
    `md5 xxxxx.xxx`

11. Encrypted Zip
    `zip -er output.zip filesource`

12. Build Folder File Tree
    
    ```
    brew install tree
    tree xxxxx
    ```

13. Customize Finder Window Size
    
    ```
    1. Open a new Finder window, do not navigate to any folders yet;
    2. Resize the window to the size you want *(however don't move the window to your desired location yet)*;
    3. start by pressing the Command ⌘ **and** Alt / Option keys together **and** drag the window to your desired location;
    4. release your mouse button first then release the Command ⌘ AND Alt / Option keys second;
    5. Close resized window;
    
    ```



14. 
