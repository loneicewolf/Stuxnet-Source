# Stuxnet-Source

### related:
- [Fanny.bmp - the Precursor to STUXNET](https://github.com/loneicewolf/fanny.bmp)

- [Gauss](Https://github.com/loneicewolf/Gauss-Src)
- [Stars](https://github.com/loneicewolf/Stars-virus)
- [Duqu](https://github.com/loneicewolf/DUQU)
- [FlamER](https://github.com/loneicewolf/flame-sourcecode)


#### right now it is text and stuff all over the place; will clean it up (therefore Branch #2)
[2nd branch](https://github.com/loneicewolf/Stuxnet-Source/tree/2022_clean)



## MAJOR UPDATE: 
will soon update this one with a live-demo of a simulated PLC workstation, which will be infiltrated(as a first step) (offline; (airgapped)) with fanny.bmp and then StuxNet; (and; why not infect it with gauss/duqu/regin and flame as well??) and try it on different types (64 bit; 32 bit; win xp; vista; ...)
even though it (was designed) to just work on 1 specific thing; which had one specific PLC-config-block(you name it); it would do some;things like mark the system "don't infect this one; this is not the correct target" or.. "don't re infect this system; I am on it"-StuxnetWorm (how it *probably* reasoning)

anyway; Will do this after my OSCP exam is passed;
and when I verified I really do have the knowledge; not just 'passing'. But for this repo I will update it just after I have passed my OSCP exam.

please; contact me for further details. mail and discord can be found on my Github Profile.


**`will clean this up later.`**

```

```
-------------------------

```

```

Old "update" message.
--- - Recording (From scratch(0%), to 100%) of when StuXnet infects a PLC (although a virtual one, since I have not *real* access to a nuclear reactor.. For.. well, quite - **obvious reasons.**
 - Recording (again, From 0 to 100%)  of how one can "re-weaponize" Fanny.bmp (or,DementiaWheel as it's codename suggests) the USB-Backdoor to carry commands from & to Metasploit. (This is tested and, let's just say - it works, but needs improvement. (Massive improvements that is)) <- Still working on it.
 - A mini-library written in C (in combination with Lua) to make (the 2 points above ) a **bit** more user-friendly 
 -    (JUST so you don't need to be a debugger-professional to understand how to get a reverse shell trough fanny's USB Backdoor for example.)
---



                                                  *(Password below), on last line*

- **(directly)** Related to fanny.bmp https://github.com/loneicewolf/fanny.bmp
- (Not directly - but *somehow*) Related: Agent.btz (finally!) added binary sample:  (more coming) https://github.com/loneicewolf/Agent.btz

## STUXNET
*is a Worm that attacked Nuclear Power plants, trough unusual vulnerabilities. So-called 0Day vulnerabilities.*

## Basic Overview:

Includes:
- Source files,
- Binaries,
- PLC Sample program

---

### fanny.bmp - (malware) what is it?
- Fanny (known as fanny.bmp or, the classical a,b,c,d,e,...,__j__.lnk worm,(Is (likely) **not ** visible in Windows XP and such, (but I have seen some versions of it where it has a,b and c - all the way up to j)- on other versions of Windows.  

- Propagates trough Removable USB devices, which has a extremely sophisticated Rootkit, which not only hides itself, but adds itself at startup in the reg in windows machines, but it has also some other, quite shocking capabilities, such as a submodule to re-program hardware, (more specifically, HDD's Firmware) for **Extreme persistence.**)
   It exploited same vulns as Stuxnet did, and has striking similarities with it, and was used **before even Stuxnet was used**)
   
   Link to fanny.bmp: https://github.com/loneicewolf/fanny.bmp
  
- Flame( Aka, SKyWiper, Flame, FlameR!, PROPS_FLAME)
- https://www.zdnet.com/article/five-years-after-the-equation-group-hdd-hacks-firmware-security-still-sucks/
- https://www.wired.com/2015/02/nsa-firmware-hacking/
- https://www.theregister.com/2015/02/17/kaspersky_labs_equation_group/

## TREE OVERVIEW  ###
Overview of Files in FILES.ZIP

---


STUXNET.DLL_EMBEDDED_RSRCS:

    bin201.bin
    bin202.bin
    bin203.bin
    bin205.bin
    bin208.bin
    bin209.bin
    bin210.bin
    bin221.bin
    bin222.bin
    bin240.bin
    bin241.bin
    bin242.bin
    bin250.bin

---


STEP7:

---


    STL-cheat-sheet-by-category.pdf -'STL-cheat-sheet-by-alphabet (1).pdf'
    S_ST70_XX_00030V.TIF
    SIMATIC_STEP7_Basic_software.jpg
    HW_e.gif
    25209116_STEP7Example.zip

---


BINS:

---


    '~WTR4141_J_37FC7C5D89F1E5A96F54318DF1A2B905.dll'
    wincc_kernel32.dll.aslr.00013b86.livebin.exe
    unknown_hook_in_services_memorymod-0x006b0000-0x006b1000.livebin.exe
    S_D102BDAD06B27616BABE442E14461059
    R_98FBEBD8883021FBE6464C37ACF17938
    Q_C1CB4117D9998C79AE10C1B890C23A4D
    P_F9BAE53E77B31841235F698955AECE30.dll
    O_CC1DB5360109DE3B857654297D262CA1.dll
    N_CA9EABEAB482524E5797C684398335D5
    mrxnet.sys.livebin.exe
    mrxnet.sys.593503354.mapped.livebin
    mrxcls.sys.livebin.exe
    mrxcls.sys.1278394761.mapped.livebin
    memorymod-pe-0x10000000-0x10138000.1155327658.mapped.livebin
    memorymod-pe-0x00090000-0x0010a000.1990061290.mapped.livebin
    memorymod-0x006b0000-0x006b1000.450210202.mapped.livebin
    maindll_dropper_memorymod-pe-0x10000000-0x10138000.livebin.exe
    M_1E17D81979271CFA44D471430FE123A5
    lsass.exe.1373553098.mapped.livebin
    lsass2_memorymod-pe-0x00090000-0x0010a000.livebin.exe
    lsass1_lsass.exe.livebin.exe
    L_4589EF6876E9C8C05DCF4DB00A54887B
    kernel32.dll.aslr.00013b86.1616636409.mapped.livebin
    K_055A3421813CAF77E1387FF77B2E2E28
    I_F8153747BAE8B4AE48837EE17172151E
    H_A3844A1B6BEA3F6FAF9C276858F40960
    G_F979C6A3E668C5073C4C6506461B034E
    F_335707EABBE7FF256E0650432ACCEC9B
    E_789F6F8DE3F140CF5D73BEF0B8ABAF78
    desktop.ini
    D_7A4E2D2638A454442EFB95F23DF391A1
    C_016169EBEBF1CEC2AAD6C7F0D0EE9026
    B_74DDC49A7C121A61B8D06C03F92D0C13
    'A_30DF51C9F0D9B010350DC09ABE1E4E97.ex$'


---



**ONLY FOR ACADEMICAL RESEARCH AND EDUCATIONAL PURPOSES**


-----------------------------------------

**If you do not know what you are doing here, now would be a great time to leave!**
(Only proceed if you **do know** what you are doing)

---



**Please Be careful with this. This is only for research and Educational Purposes.**
- **Nevertheless It goes without saying that even if you run these in a Virtual Machine, I would [still] USE CAUTION.**

---

## Password:
INFECTEDIKNOWWHATIAMDOING
