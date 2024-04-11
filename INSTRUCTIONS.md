# instructions for making and infecting a system.

# ❕ Important
When I say "Set the info" like "Set the language" or "set the time/date" I mean, set the "information"(whatever that might be) set to the particular country that was being infected the most. Like, in this case, stuxnet, Natanz, so set the country to be IRAN, the language to be, iran's main language(Persian I think, not sure), timezone, etc. etc.
Why this? it makes the system look like it's in Iran, hence increasing the probability that it might be infected, and "more properly infected" not just "infected to spread **to** **iran**")

## Cases is explained below;

`Case #1`
- using a real Windows XP laptop, (why did I chose laptop? Because that would be most easily "infect"able, laptops are carried, etc. etc.) this was Probably one of the main vectors in.


`Case #2` A bit more difficult, doable I guess but, more challenging.
- using a virtualized Windows XP (QEMU/KVM)
- make sure it's not detected at least not easily detected, that it's a VM.

both cases needs:
- care taken when creating it. How? the following to the specific malware
-  (I.e stuxnet infected Natanz so, Iran <- make it look like the system is located in Iran/Natanz) Just a example:
  - Time & Date set (Time, Date, Timezone, and time-update-settings, and time/date-display settings)
  - Geo set (Country, etc)
  - Language set
  - the system should probably be used, to some 
  - characteristics of Natanz Systems (usernames in the right language, used, etc.)
  
  -  The system should be insecure, even if stuxnet for example, uses exploits that is in windows, like bugs, it should still be easier to infect the system, so,
    -  disable:
        - firewall
        - antivirus
        - update/patches

* Dont make the system "look" too promising either cuz some malware(may or may not be stuxnet, I am not sure)  might see that and decide to maybe infect but not really go full out.
- Have some PLC Files present (included in the repo)
- Maybe try to infect using fanny.bmp too, to see so that it works. Why? cuz it's 2 related malwares(if its stuxnet and fanny that is) they are related. So maybe one of them would "help" the other malware. I.E if you have trouble infecting from scratch, stuxnet, you could* try fanny first.



---
- Q: How to transfer malware to a victim system for analysis?
- A: 3 ways I know of:
1. USB (IRL) if VM, then: (Pass the USB trough to the VM `[`in e.g QEMU/KVM`]` you can do it via the `virt-manager` )
2. HTTP (`Linux: python3 -m SimpleHTTPServer 4444` and then on `Windows: cmd.exe or internetexplorer (linux_ip:linux_port/malware.zip)`)
3. SMB (`Linux: todo`, `Windows: todo`)
4. Drag N Drop (VM)


