# ThinkPad A285 Hackintosh

 **Thanks to Collin8000 for T14 Gen1 /Efi folder which used as base for this setup**

## 📝 Specifications

| Component             | Detail                  |
|-----------------------|-------------------------|
| **CPU**               | Ryzen 5 2500U           |
| **GPU**               | Vega 8                  |
| **RAM**               | 16GB                    |
| **Motherboard**       | 20UDCTO1WW              |
| **Audio Codec**       | ALC257                  |
| **Ethernet Card**     | RTL8111                 |
| **Wifi/BT Card**      | Intel AC 9260           |
| **Touchpad Devices**  | Synaptics Touchpad      |
| **BIOS Version**      | 1.46                    |
| **Storage**           | Samsung 256gb NVME      |
| **OpenCore Version**  | 0.99                    |
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
  
</details>

<details>
<summary>❓ Not Tested</summary>

- **FindMy**
- **Dual Boot with Windows** i use arch BTW
- *...and more!*

</details>

<details>
<summary>❌ Known Issues</summary>

- **Camera**: also idk
- **BT**: idk why it's not working
- **Airdrop**: Not functioning due to Intel cards not being native, works only on Broadcom cards.
- **Screen Mirroring**: Not available unless using a paid service such as airserver.

</details>

<details>
<summary>🛠️ Post Install (Recommended)</summary>

After installing macOS, it's recommended to adjust certain settings for optimal performance:

- **iGPU Memory**: Increase the iGPU memory allocation in your BIOS settings to at least 1GB. For better performance with demanding applications, consider setting it to 2GB.
- **YogaSMC app**: Get more control over your system, Fan Control, Backlight, 

</details>


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



## 🔑 Important Information

Please note that individual results may vary. The configurations and performance can differ based on your hardware and software environments. Specifically, I have not replaced my trackpad with a glass replacement, which may not be the case for your setup. This could lead to differences in trackpad issues and performance. Use this guide as a starting point and tailor the solutions to fit your specific needs.

## 💡 Tips

- For troubleshooting, refer to the `ISSUES` tab.
- Contributions are welcome! See `CONTRIBUTING.md` for how to get started.

## 🤝 Contributions

Feel free to fork, star, and contribute to this project. Every bit of help is appreciated!

## 🙏 Acknowledgements

A shoutout to the Dortania guide and the AMD OSX Discord community for their support. And this would not have been possible without NootedRed!

## ⚠️ Disclaimer

This is a community-driven project for educational purposes. Not affiliated with Lenovo.

## Credits

- **[Apple](https://github.com/apple)**: For macOS.
- **[Dortania Guide](https://dortania.github.io/getting-started/)**: For their invaluable detailed OpenCore guide.
- **[acidanthera](https://github.com/acidanthera)**: For their OpenCore bootloader and essential kexts that make running macOS on X86 possible.
- **[Baio1977](https://github.com/Baio1977)** and **[Askwakhid](https://github.com/askwakhid)**: For both of their Hackintosh EFI posts about the intel version of the T14. Another thanks to Baio1977 for the bios section of this post
