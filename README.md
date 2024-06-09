# ThinkPad A285 Hackintosh

 **I've found that this repo was cloned on the pudn.com by "sh-1993", so, I should say that this config made by da1la on github**

## 📝 Specifications

| Component             | Detail                  |
|-----------------------|-------------------------|
| **CPU**               | Ryzen 5 2500U           |
| **GPU**               | Vega 8                  |
| **RAM**               | 16GB                    |
| **Motherboard**       | 20MXS07A00              |
| **Audio Codec**       | ALC257                  |
| **Ethernet Card**     | RTL8111                 |
| **Wifi/BT Card**      | Intel AC 9260           |
| **Touchpad Devices**  | Synaptics Touchpad      |
| **BIOS Version**      | 1.47                    |
| **Storage**           | Intel 256gb NVME        |
| **OpenCore Version**  | 0.9.9                   |
| **Device**            | Thinkpad A285           |

## 💻 Supported macOS Versions

- **Sonoma**: Installs, fully works
- **Ventura**: Potential support, not installed.
- **Monterey**: Not tested and supported.

<details>
<summary>✅ What's Working</summary>

- **WIFI**
- **Trackpad**
- **Battery Status**
- **Backlight**
- **IGPU**
- **Fan Control**: Full YogaSMC EC Access.
- **FN keys**
- **Audio**
- **Camera**: fixed after USB mapping
- **BT**: also fixed
- **Dual Boot with Windows**: just for USB remap
- *...and more!*
  
</details>

<details>
<summary>❌ Known Issues</summary>

- **WWAN**: i don't have one, and mac os not support that anyway
- **sleep**: I'm working about that
- **Airdrop**: Not functioning due to Intel cards not being native, works only on Broadcom cards.
- **Screen Mirroring**: Not available unless using a paid service such as airserver.

</details>

<details>
<summary>🛠️ Post Install (Recommended)</summary>

After installing macOS, it's recommended to adjust certain settings for optimal performance:

- **iGPU Memory**: Increase the iGPU memory allocation in your BIOS settings to at least 1GB.
- **YogaSMC app**: Get more control over your system, Fan Control, Backlight, 

</details>

<details>
<summary>⚙️ BIOS Settings (Mandatory)</summary>

To ensure your Hackintosh functions correctly, configure the following mandatory BIOS settings:

**Config Tab:**
- Display
  - Boot Display Device -> Thinkpad LCD
  - Shared Display Priority -> HDMI
  - Boot Time Extension -> Disabled

**Security Tab:**
- Memory Protection -> Execution Prevention -> On

**Startup Tab:**
- UEFI/Legacy Boot -> UEFI Only

These settings are crucial for the proper operation of your Hackintosh system.
</details>

</details>



## 🔑 Important Information

Potentially it can work on that laptops:

- Thinkpad A485
- Thinkpad X395 (not sure, better see [That project](https://github.com/adam-ht/Lentosh))
- Thinkpad E485
- Thinkpad E585
- IdeaPad 330-15ARR
- IdeaPad 720S-13ARR
- Yoga 530-14ARR

**BUT** it'll require USB remapping **AND** generating ACPI tables.
I've used this guides:
- https://www.reddit.com/r/hackintosh/comments/ta1ef4/guide_easy_usb_mapping_with_usbtoolbox_on_windows/
- https://chefkissinc.github.io/guide/gathering-files/acpi

## 🤝 Contributions

Feel free to fork, star, and contribute to this project. Every bit of help is appreciated!

## 🙏 Acknowledgements

A shoutout to the Dortania guide and the AMD OSX Discord community for their support. And this would not have been possible without NootedRed!

## ⚠️ Very important

I use Arch BTW

## Credits
- **[shipasnake](https://github.com/da1la)**: (me) For creating that project
- **[Collin8000](https://github.com/Collin8000/Thinkpad-T14-Gen-1-Amd-Hackintosh)**: For Thinkpad T14 G1 efi folder
- **[Apple](https://github.com/apple)**: For macOS.
- **[Dortania Guide](https://dortania.github.io/getting-started/)**: For their invaluable detailed OpenCore guide.
- **[acidanthera](https://github.com/acidanthera)**: For their OpenCore bootloader and essential kexts that make running macOS on X86 possible.
- **[Baio1977](https://github.com/Baio1977)** and **[Askwakhid](https://github.com/askwakhid)**: For both of their Hackintosh EFI posts about the intel version of the T14. Another thanks to Baio1977 for the bios section of this post
