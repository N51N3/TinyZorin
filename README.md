# ⚠️ Important Notice ⚠️

> **A clean and updated version of this document is published on my website:**
>
> **🌐 [https://n51n3.bearblog.dev/tinyzorin](https://n51n3.bearblog.dev/tinyzorin)**

I am an absolute Linux beginner, and this is a living document constantly updated with the new things I've learnt and done on my freshly installed ZorinOS to guide other new beginners to improve their Linux Installation.

You're encouraged to do these two things;  
- Follow & share feedback for this project on [Telegram](https://t.me/+eeX3S3cAm9A5ZDQ0)
- Star & share this project

## Get Started  
Do the following first on your computer;

<details>  
  <summary>Prerequisite</summary>  
  <ul>
    <li>Check system requirement & hardware compatibility <a href="https://help.zorin.com/docs/getting-started/system-requirements">here.</a></li>  
    <li>Backup your files in an external drive</li>
  </ul>  
</details>  

<details>  
  <summary>Install ZorinOS</summary>  
  <ul>  
    <li>Follow this guide on <a href="https://help.zorin.com/docs/getting-started/install-zorin-os/">how to install ZorinOS.</a></li>
    <li>For visual learners, here's a <a href="https://www.youtube.com/watch?v=sA3igThg1qc">video guide</a></li>    
  </ul>  
</details>
 

## Update Installations  
After installation, update everything to the latest version through Zorin's GUI or copy the commands and run them in Terminal;  

<details>  
  <summary>System Update</summary>  
  <ul>  
    <li>Open the <strong>Software Store</strong> and click on <strong>Updates</strong> >> <strong>Update All</strong></li> 
    <li>Still on the same page, click on <strong>Main Menu</strong> >> <strong>System Respositories</strong> then turn on <strong>Canonical-supported free and open source software</strong>.</li>
    <li>A pop-up will appear. Click <strong>Close</strong></li>
  </ul>  
</details>  

<details>  
  <summary>Update Through Terminal</summary>  
   <ul>  
    <li>Open the Termimal app and paste these commands;</li>
    <li><code>sudo apt update</code> + <code>enter</code> to check for updates</li>
    <li><code>sudo apt upgrade</code> + <code>enter</code> to apply the updates</li>
    <li><code>sudo ubuntu-drivers autoinstall</code> + <code>enter</code> to install proprietary drivers</li>
    <li>Restart your computer</li>
  </ul> 
</details>  
 
<details>  
  <summary>Update Drivers</summary>   
  <ul>
    <li>Open the <strong>Software Store</strong> and click on <strong>Main Menu</strong></li>  
    <li>Click on <strong>System Respositories</strong></li>
    <li>Click on <strong>Additional Drivers</strong> then <strong>Update</strong></li> 
    </ul>
</details>  

<details>  
  <summary>Update GPU Driver(Intel/AMD)</summary>   
  <ul>  
    <li>Check if your laptop has the <strong>Mesa Intel® Xe Graphics (TGL GT2)</strong></li>  
    <li>Open the Termimal app and paste this command to update it;</li>
    <li><code>sudo apt install mesa-utils</code> + <code>enter</code> to check for updates</li>
  </ul>
</details>

## System Optimization  
Settings to Improve performance, efficiency, and overall functions of your computer.  

<details>  
  <summary>Intall Ubuntu Restricted Extras</summary>  
  <ul>  
    <li>This enables support for a wide range of multimedia formats and proprietary tools like audio and video codecs, Adobe Flash Plugin, Unrar and GStreamer Plugins on your computer</li>
    <li><code>sudo apt install ubuntu-restricted-extras</code> + <code>enter</code> to install</li>  
 </ul> 
</details>  

<details>  
  <summary>Reduce Boot Time</summary>  
  <ul>  
    <li>This disables the network wait service, which can slow down boot times.</li>
    <li><code>sudo systemctl disable NetworkManager-wait-online.service</code> + <code>enter</code> to install</li>  
 </ul> 
</details>

<details>  
  <summary>Enable zswap for Better RAM Management</summary>  
  <ul>  
    <li>This helps improve performance on systems with limited RAM</li>
    <li><code>echo "zswap.enabled=1" | sudo tee -a /etc/default/grub && sudo update-grub</code> + <code>enter</code> to install</li>  
 </ul> 
</details>  

<details>  
  <summary>Enable Fractional Scaling (for High-DPI Displays):</summary>  
  <ul>  
    <li>This makes fonts and UI elements look sharper on high-resolution screens.</li>
    <li>gsettings set org.gnome.mutter experimental-features "['scale-monitor-framebuffer']"</code> + <code>enter</code> to install</li>  
 </ul> 
</details> 

## Install Apps & Packages  
ZorinOS comes with a built-in Software Store and here are packages with beautiful UIs that I use and recommend;  
<details>  
  
  <summary>Zen</summary>  
    <ul>   
      <li>A minimalist, lightweight open-source browser based on FireFox with a vertical tab bar.</li>
      <li>Download from the software store</li>
    </ul> 
</details>  

<details>  
  <summary>Keypunch</summary>  
    <ul>   
      <li>A minimalist app to practise and improve your typing skills</li>
      <li>Download from the software store</li>
    </ul> 
</details>  

<details>  
  <summary>Diodon</summary>  
    <ul>   
      <li>A simple clipboard manager</li>
      <li>Download from the software store</li>
   </ul> 
</details>  

<details>  
  <summary>OCRFeeder</summary>  
    <ul>   
      <li>An app that allows you copy text from images</li>
      <li>Download from the software store</li>
   </ul> 
</details>
