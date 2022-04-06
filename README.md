# AERIN's Enchiridion 
|> Why would you want to lower and stabilize the latency of your hardware?
|> A consistent feeling is critical for most competitively played games as your entire gameplay relies on it
|> Sudden increase in latency/instability/insane DPM downclocking = worsened latency, you miss the shot thats responsible for having you on a leaderboard
|> Can you actually feel these few milliseconds? Yes, you definitely can.

https://www.nvidia.com/en-us/geforce/news/reflex-low-latency-platform/#why-does-system-latency-matter
https://www.youtube.com/watch?v=vOvQCPLkPt4&t=80s&ab_channel=MicrosoftResearch
https://www.youtube.com/watch?v=muvToLXJSks&ab_channel=NVIDIAGeForce

# Frames and other useless metrics
|> "You can always increase bandwidhh but you cannot ask God to increase the speed of light"
|> Nothing but 0.1% frames matter, and even these cannot always be used as a reliable metric
|> Bandwidth is a joke, focusing on it is the reason we still use memory with 80% unnecessary latency

# Mainstream marketing and other scams
|> Pre-built computers and other such scams wouldn't exist if people would buy hardware with focus on performance
|> RGB/looks of a dont matter (Do you seriosuly think you'll look at your display or at your pc while playing and/or working?), yet thats what the current market is focused on. Such consumer hardware can be bought for insanely cheap and it's sure to sell due to a specific component/aspect (E.g.: $80 CPU, $25 RAM, air cooling, server board BUT with a 3080 and RGB = Will always sell out instantly (and perform worse than a $500 build due to various stutters and the GPU being 500% too strong for anything else within said machine))
|> Hardware designed for workstations is sold to you for gaming and said to perform well while affecting the entire system due it's architecture/latency
|> (Ryzen, NVIDIA = FOR WORKSTATIONS AND COMPUTING TASKS, NOT GAMING)

# Low latency hardware

CPUS
|> Ryzen will not be mentioned again as it's incapable of RAM overclocking beyond 1900 FCLK (FCLK = 1/2MCLK) and it's IMC falls without aditional stability settings such as GDM
|> 9900K, 10900K, 12900K
|> 10900K may not prove perfect stability at all times, thus 9900K/12900K should be the first choice

Motherboards
|> For Coffee Lake: Z390 DARK (Buy used from ebay, you will not find unused ones. Goes for $350-$500)
                    Z390 Apex XI (A good choice if you can't find a DARK. Similar price)
                    Z390i (If you really need a new board and can't afford #1 & #2, get one of these. Anything besides Gigabyte will do just fine)

|> For Comet Lake: Z490 Dark ($450-$600)
                   Z390 Apex XI (A good choice if you can't find a DARK. $350)
                   Z490i Unify (Great third choice, keep your NIC in mind. Board also has standard ATX version. $250)
                   Z490i (As long as it's not a Gigabyte one it'll be "good enough" if you need a decent board <$250)
               
|> For Alder lake: Z690 Asus Rog DDR4 ($300)
                   Z690 Asus Tuf Gaming DDR4 ($300, slightly worse than ROG)
                   Z690 Msi Pro DDR4 ($200, direct phase but disgusting firmware, only recommended as the very last option)
                   
CPU Coolers
|> Arctic Liquid Freezer ii 280mm (or 360/420) combined with Thermal Grizzly Kryonaut, possible even Conductonaut if delidded ($80)

RAM
|> Always buy G.Skill Ripjaws V Black. Theyre cheaper than Trident kits and usually perform just the same while being B-die
|> Do NOT buy Corsair RAM due to it utilising a EFM8UB20F64G-B-QFP32 bootloader (which it can be disabled by writing a non-0xA5 to it's signature)
|> Buy dual rank (2x16GB) if your board works well with it 
|> Remove heatsinks by heating them up with a hairdryer and using a knive to strip each side away
|> Use at least 1 fan on your RAM and keep it below 36c when during stress testing
|> Don't buy 3600 16 16 as it may end up being C-die
|> Decent kits that you can find as single and dual rank are: 4000 14 15
                                                              4266 16 16
                                                              3600 14 15
                                                              3200 14 14

Power supplies
|> Ripple affects all other parts so that'll be the judge of PSU quality
|> Ax1600 with proper AC cables above all others 
|> RM1000x, RM850x, RM750x will do just fine in a non-professionally used build

NIC's
|> XG-C100C
|> X550T2
|> I210T1

Routers
|> XR-300 abve all other ones
|> Flash openWRT to get rid of certain mitigations, set up QoS and disable Wi-Fi (it affects you/your hardware/your cables/everything)

Monitors
|> Don't buy IPS or VA panels, only twisted nematic (TN)
|> XV252QF
|> HP OMEN x25 (non -F version)
|> VG258QM
|> Max out overdrive and enable all settings that improve response time
|> Disable/lower all color/image quality settings as much as possible
|> Disable DDC/Ci
|> Delete all EDID's besides a custom one with 6BPC, static pixel clock and timings
|> Use 1600x900 if your display has a good scaler

# Graphics Cards
|> AMD POLARIS10 ABOVE ALL OTHER ONES <|
|> AMD GPU's have 10x+ more interrupts than NVIDIA
|> AMD has better rasterization by default
|> AMD GPU's must be backed up by proper hardware, even the best of RAM can barely keep up with them
|> Use the Linux Api to recreate your entire card or purchasing a such GPU's is not worth it for you
|> Games that utilies Unreal Engine are optimized for NVIDIA, so expect less 'frames' on AMD unless optimized to the very end
|> NVIDIA's frame scams with tiling, memory timings and compute optimization exist because they sell consumer hardware
|> Lock your clocks, voltages and fan speeds via SPPT/VBIOS/NvAPI/Linux Api/NvPowerAPI/etc. (otherwise your GPU will constantly downclock due to DPM and power states
|> NVIDIA does not require a shunt mod for increased power limits, contrary to popular belief.
|> Use Thermal Grizzly Kryonaut oder Conductonaut and replace stock shroud with Noctua DC/Phanteks T30 fans
|> Disable all RGB lights by unplugging all JW from your GPU
|> BIOS settings affect PCIE>GPU
|> Registry keys can override (V-)BIOS settings
|> 1% improvement in PCIE RX/TX latency is worth 10 RAM ns

# BIOS
|> Every BIOS has a few thousand settings hidden from consumers
|> Disable BCLK SSC if it's visible, otherwise use the GRUB bootloader oder AmiSceWin/AmiSceEfi
|> Disable all other SSC, they affect all clocks
|> Disable selfrefresh (it will break shutdowns/reboots but it's worth it, just wire your POWER_SW to a button and you're good to go)
|> Disable Rowhammer
|> Disable hyperthreading/simultaneous threading control (SMT), C-States, RAM powerdown, Intel Turbo 
|> Disable all other powersaving and unused ports/slots/connectors
|> Change RAM timings that aren't visible within your BIOS
|> 


# UPDATING SOON//







