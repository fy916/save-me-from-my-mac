# save-me-from-my-mac

A collections of utility scripts or commands I write and gather to enhance macos experience





1.  Adjust MacOS menubar padding 
   `defaults -currentHost write -globalDomain NSStatusItemSelectionPadding -int 8`



2. Time Machine Speed Up
   `sudo sysctl debug.lowpri_throttle_enabled=0`
   

3. Delete Local Snapshots (when deleting files does not release space)

4. `for d in $(tmutil listlocalsnapshotdates | grep "-"); do sudo tmutil deletelocalsnapshots $d; done`



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
    
    `brew install tree`
    
    `tree xxxxx`
