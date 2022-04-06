# AERIN's Enchiridion 
* Why would you want to lower and stabilize the latency of your hardware? <br />
* A consistent feeling is critical for most competitively played games as your entire gameplay relies on it <br />
* Sudden increase in latency/instability/insane DPM downclocking = worsened latency, you miss the shot thats responsible for having you on a leaderboard <br />
* Can you actually feel these few milliseconds? *Yes, you definitely can.* <br />
* [My twitter](https://twitter.com/aerin0x01)


https://www.nvidia.com/en-us/geforce/news/reflex-low-latency-platform/#why-does-system-latency-matter <br />
https://www.youtube.com/watch?v=vOvQCPLkPt4&t=80s&ab_channel=MicrosoftResearch <br />
https://www.youtube.com/watch?v=muvToLXJSks&ab_channel=NVIDIAGeForce <br />

# Frames and other useless metrics
* *"You can always increase bandwidth but you cannot ask God to increase the speed of light"* <br />
* Nothing but 0.1% frames matter, and even these cannot always be used as a reliable metric <br />
* Bandwidth is a joke, focusing on it is the reason we still use memory with *80% unnecessary latency* <br />

# Mainstream marketing and other scams
* Pre-built computers and other such scams wouldn't exist if people would buy hardware with focus on performance <br />
* RGB/looks of a dont matter (Do you seriosuly think you'll look at your display or at your pc while playing and/or working?), yet thats what the  current market is focused on. Such consumer hardware can be bought for insanely cheap and it's sure to sell due to a specific component/aspect (E.g.: $80 CPU, $25 RAM, air cooling, server board BUT with a 3080 and RGB = Will always sell out instantly (and perform worse than a $500 build due to various stutters and the GPU being 500% too strong for anything else within said machine)) <br />
* Hardware designed for workstations is sold to you for gaming and said to perform well while affecting the entire system due it's architecture/latency <br />
* (Ryzen, NVIDIA = FOR WORKSTATIONS AND COMPUTING TASKS, NOT GAMING) <br />

# Low latency hardware

**CPUS**
* Ryzen will not be mentioned again as it's incapable of RAM overclocking beyond 1900 FCLK (FCLK = 1/2MCLK) and it's IMC falls without aditional stability settings such as GDM <br />
* 9900K, 10900K, 12900K <br />
* 10900K may not prove perfect stability at all times, thus 9900K/12900K should be the first choice <br />

**Motherboards**
* For Coffee Lake: Z390 DARK (Buy used from ebay, you will not find unused ones. Goes for $350-$500) <br />
                    Z390 Apex XI (A good choice if you can't find a DARK. Similar price) <br />
                    Z390i (If you really need a new board and can't afford #1 & #2, get one of these. Anything besides Gigabyte will do just fine) <br />

* For Comet Lake: Z490 Dark ($450-$600) <br />
                   Z390 Apex XI (A good choice if you can't find a DARK. $350) <br />
                   Z490i Unify (Great third choice, keep your NIC in mind. Board also has standard ATX version. $250) <br />
                   Z490i (As long as it's not a Gigabyte one it'll be "good enough" if you need a decent board <$250) <br />
               
* For Alder lake: Z690 Asus Rog DDR4 ($300) <br />
                   Z690 Asus Tuf Gaming DDR4 ($300, slightly worse than ROG) <br />
                   Z690 Msi Pro DDR4 ($200, direct phase but disgusting firmware, only recommended as the very last option) <br />
                   
**CPU Coolers**
* Arctic Liquid Freezer ii 280mm (or 360/420) combined with Thermal Grizzly Kryonaut, possible even Conductonaut if delidded ($80) <br />

**RAM**
* Always buy G.Skill Ripjaws V Black. Theyre cheaper than Trident kits and usually perform just the same while being B-die <br />
* Do NOT buy Corsair RAM due to it utilising a EFM8UB20F64G-B-QFP32 bootloader (which can be disabled by writing a non-0xA5 to it's signature) <br />
* Buy dual rank (2x16GB) if your board works well with it  <br />
* Remove heatsinks by heating them up with a hairdryer and using a knive to strip each side away <br />
* Use at least 1 fan on your RAM and keep it below 36c when during stress testing <br />
* Don't buy 3600 16 16 as it may end up being C-die <br />
* Decent kits that you can find as single and dual rank are: 4000 14 15 <br />
                                                              4266 16 16 <br />
                                                              3600 14 15 <br />
                                                              3200 14 14 <br />

**Power supplies**
* Ripple affects all other parts so that'll be the judge of PSU quality <br />
* Ax1600 with proper AC cables above all others  <br />
* RM1000x, RM850x, RM750x will do just fine in a non-professionally used build <br />

**NICs**
* XG-C100C <br />
* X550T2 <br />
* I210T1 <br />

**Routers**
* XR-300 abve all other ones <br />
* Flash openWRT to get rid of certain mitigations, set up QoS and disable Wi-Fi (it affects you/your hardware/your cables/everything) <br />

**Monitors**
* Don't buy IPS or VA panels, only twisted nematic (TN) <br />
* XV252QF <br />
* HP OMEN x25 (non -F version) <br />
* VG258QM <br />
* Max out overdrive and enable all settings that improve response time <br />
* Disable/lower all color/image quality settings as much as possible <br />
* Disable DDC/Ci <br />
* Delete all EDID's besides a custom one with 6BPC, static pixel clock and timings <br />
* Use 1600x900 if your display has a good scaler <br />

**Graphics Cards**
* AMD POLARIS ABOVE ALL OTHER ONES <br />
* AMD GPU's have 10x+ more interrupts than NVIDIA <br />
* AMD has better rasterization by default <br />
* AMD GPU's must be backed up by proper hardware, even the best of RAM can barely keep up with them <br />
* Use the Linux Api to recreate your entire card or purchasing a such GPU's is not worth it for you <br />
* Games that utilies Unreal Engine are optimized for NVIDIA, so expect less 'frames' on AMD unless optimized to the very end <br />
* NVIDIA's frame scams with tiling, memory timings and compute optimization exist because they sell consumer hardware <br />
* Lock your clocks, voltages and fan speeds via SPPT/VBIOS/NvAPI/Linux Api/NvPowerAPI/etc. (otherwise your GPU will constantly downclock due to DPM and power states <br />
* NVIDIA does not require a shunt mod for increased power limits, contrary to popular belief <br />
* Use Thermal Grizzly Kryonaut oder Conductonaut and replace stock shroud with Noctua DC/Phanteks T30 fans <br />
* Disable all RGB lights by unplugging all JW from your GPU <br />
* BIOS settings affect PCIE>GPU <br />
* Registry keys can override (V-)BIOS settings <br />
* 1% improvement in PCIE RX/TX latency is worth 10 RAM ns <br />

**BIOS**
* Every BIOS has a few thousand settings hidden from consumers <br />
* Disable BCLK SSC if it's visible, otherwise use the GRUB bootloader oder AmiSceWin/AmiSceEfi <br />
* Disable all other SSC, they affect all clocks <br />
* Disable selfrefresh (it will break shutdowns/reboots but it's worth it, just wire your POWER_SW to a button and you're good to go) <br />
* Disable Rowhammer <br />
* Disable hyperthreading/simultaneous threading control (SMT), C-States, RAM powerdown, Intel Turbo <br />
* Disable all other powersaving and unused ports/slots/connectors <br />
* Change RAM timings that aren't visible within your BIOS <br />
*  <br />


# UPDATING SOON//







