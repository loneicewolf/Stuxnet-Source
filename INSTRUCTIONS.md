# Instructions for Creating and Infecting a System

## ❕ Important
When configuring the system, ensure that you set the information (such as language, time/date, and region) to match the target country of the malware. For example, in the case of Stuxnet, which targeted Natanz in Iran, set the system's location, language (Persian), and timezone to reflect Iran. This configuration helps to make the system appear as if it is genuinely located in the target region, thereby increasing the likelihood of successful infection.

## Cases

### Case #1: Physical Windows XP Laptop
- **Description**: Using a real Windows XP laptop, which might have been a primary infection vector due to its portability.
- **Reasoning**: Laptops are more easily transported and used in various locations, which could contribute to their role in spreading malware.

### Case #2: Virtualized Windows XP
- **Description**: Using a virtualized environment (e.g., QEMU/KVM) for Windows XP.
- **Challenge**: Ensure the virtual machine is not easily detectable as a VM to prevent detection by the malware.

### Common Requirements for Both Cases
- **System Configuration**: 
  - Set the time, date, timezone, and date/time display settings to match the target region (e.g., Iran).
  - Configure the geo-location settings (country, language) to reflect the target.
  - Adjust system settings to mimic the characteristics of the target environment (e.g., use relevant usernames and settings).

- **System Security**: 
  - Disable security features to make the system more vulnerable:
    - **Firewall**
    - **Antivirus**
    - **System Updates/Patches**

- **Additional Considerations**:
  - **PLC Files**: Include relevant PLC files (available in the repository) to enhance the authenticity of the setup.
  - **Dual Malware Test**: Optionally, try infecting the system using Fanny.bmp in addition to Stuxnet. This might help in understanding if the presence of one malware could assist in the infection process of the other.

## Transferring Malware to the Victim System
Here are several methods to transfer malware to the system for analysis:

1. **USB**: For physical systems, use a USB drive. For virtual machines, pass the USB through to the VM (e.g., via `virt-manager` in QEMU/KVM).
2. **HTTP**: Host the malware on a local HTTP server (`Linux: python3 -m http.server 4444`) and download it from the Windows VM using `cmd.exe` or a browser (`linux_ip:linux_port/malware.zip`).
3. **SMB**: Transfer files over SMB (setup instructions needed for both Linux and Windows).
4. **Drag and Drop**: If using a VM, drag and drop the files directly into the VM environment.

## Tools
- [Kernel Detective](https://github.com/Fyyre/kerneldetective)
- [DrvMon](https://github.com/Fyyre/DrvMon)
- [Crypto Utils](https://github.com/hasherezade/crypto_utils)

---

Please ensure that all activities are performed in a controlled environment and follow ethical guidelines for malware analysis. Proceed with caution and always prioritize safety.
