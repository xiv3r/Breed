# Router Breed
© [Pascal](breed.hackpascal.net)


[Enter Web Flashing Mode]
Set the computer network connection to automatically obtain the IP address
Open CMD and run ping 192.168.1.1 -tNote
that starting from r979, this IP address can be modified, so in actual operation, you need to replace it with the modified IP.
Press the reset button or WPS button and then power on the router. If you see some or all of the router's LEDs flash 4 times in a row, or ping is successful, it means that you have entered the Web Flashing Mode

[Enter Web Flashing Mode without pressing the reset button]
This is achieved through a Breed Enter tool (requires Npcap support)
https://github.com/nmap/npcap/releases/download/v0.10-r7/npcap-0.10-r7.exe Download Npcap, and when installing, the WinPcap compatibility mode
should support Windows XP
Click here to download the Windows XP-specific beta version of BreedEnter (compiled using WDK 7.1.0): http://breed.hackpascal.net/BreedEnter-VC80-XP.zip

Make sure the router is connected to the computer via an Ethernet cable
1. Start BreedEnter.exe

2. Power off and then power on the router

3. If the program interface prompts as follows, it means that you have entered the Web flashing mode


[Change the serial port baud rate]
Enter the Breed command console
Execute the command setbrg <baud rate>
Restart to take effect


[File description]
Breed files that are no longer updated have been moved to https://breed.hackpascal.net/EOL/ . The last revision number will be indicated after the file name.
file name	illustrate
BreedEnter.exe	Breed boot interruption tool, enter Web flashing mode without pressing reset button
md5sum.txt	MD5 values ​​of all Breed files in the current version, used to verify the integrity of the files
breed-mt7620-reset1.bin	MT7620A / MT7620N universal, baud rate 57600, reset button GPIO#1
breed-mt7620-reset2.bin	MT7620A / MT7620N universal, baud rate 57600, reset button GPIO#2
breed-mt7620-reset11.bin	MT7620A / MT7620N universal, baud rate 57600, reset button GPIO#11
breed-mt7620-reset12.bin	MT7620A / MT7620N universal, baud rate 57600, reset button GPIO#12
breed-mt7620-reset13.bin	MT7620A / MT7620N universal, baud rate 57600, reset button GPIO#13
breed-mt7620-reset26.bin	MT7620A / MT7620N universal, baud rate 57600, reset button GPIO#26
breed-mt7620-reset30.bin	MT7620A / MT7620N universal, baud rate 57600, reset button GPIO#30
breed-mt7620-rt-n14u.bin	MT7620A / MT7620N universal, baud rate 57600, reset button GPIO#1, WPS button GPIO#2
breed-mt7620-whr-1166dhp.bin	MT7620A / MT7620N universal, baud rate 57600, reset button GPIO#52, AOSS button GPIO#53
breed-mt7620-lenovo-y1.bin	Lenovo Y1 (newifi mini) dedicated, baud rate 115200, reset button GPIO#11
breed-mt7620-lenovo-y1s.bin	Lenovo Y1S (newifi) dedicated, Gigabit port available, baud rate 115200, reset button GPIO#11
breed-mt7620-zte-q7.bin	ZTE Q7 dedicated, baud rate 57600, reset button GPIO#26
breed-mt7620-youku-yk1.bin	Dedicated for Youku Router, baud rate 57600, reset button GPIO#1
breed-mt7620-xiaomi-mini.bin	Dedicated for Xiaomi Mini, baud rate 115200, reset button GPIO#30
breed-mt7620-fir302m.bin	Phicomm FIR300M/302M dedicated, baud rate 57600, reset button GPIO#2
breed-mt7620-phicomm-psg1208.bin	Phicomm PSG1208 (K1)/ PSG1218 (K2) dedicated, baud rate 57600, reset button GPIO#1
breed-mt7620-hiwifi-hc5761.bin	Dedicated for Ji Router Jiyi S (HC5661)/Jiyi Er (HC5761), baud rate 115200, reset button GPIO#12
breed-mt7620-hiwifi-hc5861.bin	Dedicated for Ji Router Ji San (HC5861), Gigabit LAN available, baud rate 115200, reset button GPIO#12
breed-mt7620-oye-0001.bin	Oye-0001 dedicated, baud rate 115200, reset button GPIO#1
breed-mt7620-airmobi-iplay2.bin	AirMobi iPlay2 dedicated, baud rate 57600, reset button GPIO#26
breed-mt7621-newifi-d1.bin	Lenovo Newifi D1 dedicated, DDR3  memory applicable, default 256MB DDR AC timing parameters, baud rate 115200, reset button GPIO#15, WPS button GPIO#18
breed-mt7621-newifi-d2.bin	Lenovo Newifi D2 dedicated, DDR3 memory applicable, default 512MB DDR AC timing parameters, baud rate 115200, reset button GPIO#3, WPS button GPIO#7
breed-mt7621-xunlei-timeplug.bin	Dedicated for Thunder Time Machine (Time Cloud), applicable to DDR3 memory, default 256MB DDR AC timing parameters, baud rate 115200, reset button GPIO#4
breed-mt7621-youku-l2.bin	Dedicated for Youku Router YK-L2, suitable for DDR3 memory, default 256MB DDR AC timing parameters, baud rate 115200, reset button GPIO#18, WPS button GPIO#17
breed-mt7621-phicomm-k2p.bin	Phicomm K2P dedicated, suitable for DDR3 memory, default 512MB DDR AC timing parameters, baud rate 57600, reset button GPIO#3
breed-mt7621-pbr-m1.bin	Dedicated for PandoraBox PBR-M1, suitable for DDR3 memory, default 512MB DDR AC timing parameters, baud rate 115200, reset button GPIO#18
breed-mt7621-totolink-a3004ns.bin	Dedicated for TOTOLINK A3004NS, suitable for DDR3  memory , default 256MB DDR AC timing parameters, baud rate 57600, reset button GPIO#4, WPS button GPIO#3
breed-mt7621-xiaomi-r3g.bin	Xiaomi router 3G dedicated, NAND boot, DDR3 memory applicable, default 256MB DDR AC timing parameters, baud rate 115200, reset button GPIO#18
breed-mt7621-creativebox-v1.bin	CreativeBox v1 dedicated, suitable for DDR3 memory, default 512MB DDR AC timing parameters, baud rate 115200, reset button GPIO#18
breed-mt7621-hiwifi-hc5962.bin	Dedicated for Jilu Router 4/HC5962/B70, NAND boot, applicable to DDR3 memory, default 256MB DDR AC timing parameters, baud rate 115200, reset button GPIO#18
breed-mt7621-r6220.bin	Netgear R6220 dedicated, NAND boot, DDR2 memory applicable, fixed 128MB DDR AC timing parameters, baud rate 57600, reset key GPIO#14, WPS key GPIO#7, RFKILL key GPIO#8
breed-mt7621-wndr3700v5.bin	Netgear WNDR3700 v5 dedicated, DDR2 memory applicable, fixed 128MB DDR AC timing parameters, baud rate 57600, reset button GPIO#14, WPS button GPIO#7, RFKILL button GPIO#8
breed-mt7621-gehua-ghl-r-001.bin	Dedicated for Gehua GHL-R-001, suitable for DDR3  memory , default 512MB DDR AC timing parameters, baud rate 57600, reset button GPIO#18
breed-mt7621-jd-cloud-1.bin	 JD Cloud Router RE-SP-01B dedicated, suitable for DDR3 memory, default 512MB DDR AC timing parameters, baud rate 115200, reset button GPIO#18
breed-mt7628-hiwifi-hc5661a.bin	Dedicated for Ji Router Jiyi S (HC5661A), baud rate 115200, reset button GPIO#38
breed-mt7628-oye-0006.bin	OYE-0006 dedicated, baud rate 115200, reset button GPIO#38
breed-mt7688-reset38.bin	MT7628AN/KN universal, baud rate 57600, reset button GPIO#38
breed-mt7688-wrtnode2r.bin	MT7628AN/KN universal, baud rate 115200, reset button GPIO#5
breed-rt3050-buffalo-wcr-hp-gn.bin	Buffalo WCR-HP-GN dedicated, SPI boot, baud rate 57600, reset button GPIO#10, WPS button GPIO#0
breed-rt3050-di-524m-b1.bin	D-LINK DI-624M B1 dedicated, SPI start, baud rate 57600, reset button GPIO#10
breed-rt305x-nor-reset0.bin	RT305X general purpose, NOR boot, baud rate 57600, reset button GPIO#0
breed-rt305x-nor-reset10.bin	RT305X general purpose, NOR boot, baud rate 57600, reset button GPIO#10
breed-rt3052-dir-605-b1.bin	D-LINK DIR-605 B1 dedicated, NOR boot, baud rate 57600, reset key GPIO#10, WPS key GPIO#0
breed-rt3052-hg255d.bin	Dedicated for Huawei HG255D, NOR boot, baud rate 115200, reset button GPIO#4, WPS button GPIO#10
breed-rt5350-airmobi-iplay.bin	AirMobi iPlay dedicated, baud rate 57600, reset button GPIO#12
breed-rt5350-hame-a5.bin	Huamei A5 dedicated, baud rate 57600, reset button GPIO#0
breed-rt5350-zm-10.bin	Zhongwo ZM-10 dedicated, baud rate 57600, reset button GPIO#10
breed-ar7161-dir-825-b1.bin	D-LINK DIR-825 B1 dedicated, baud rate 115200, reset key GPIO#3, WPS key GPIO#8
breed-ar724x.bin	AR724X Universal, 100M wired, baud rate 115200, reset button GPIO#11, QSS button GPIO#12
breed-ar724x-reset11.bin	AR724X Universal, 100M wired, baud rate 115200, reset button GPIO#11
breed-ar724x-reset12.bin	AR724X Universal, 100M wired, baud rate 115200, reset button GPIO#12
breed-ar7240-wnr1000v2.bin	Netgear WNR1000 v2 dedicated, 100M wired, baud rate 115200
breed-ar7242-wr2543nd.bin	TP-LINK WR2543ND dedicated, baud rate 115200, reset key GPIO#11, QSS key GPIO#12
breed-ar7242-aruba-ap93.bin	Aruba-AP93 dedicated, Gigabit wired, baud rate 115200, reset button GPIO#11, WPS button GPIO#12
breed-ar913x.bin	AR913X Universal, 100M wired, baud rate 115200, reset button GPIO#7, WPS button GPIO#3
breed-ar9132-wr1043ndv1.bin	TP-LINK WR1043ND v1 dedicated, baud rate 115200, reset button GPIO#7, WPS button GPIO#3
breed-ar9331.bin	AR9331 general purpose, baud rate 115200, reset button GPIO#11
breed-ar9331-mr12u.bin	TP-LINK MR12U dedicated, baud rate 115200, reset button GPIO#11
breed-ar9331-pisen.bin	PISEN Cloud Router (Cloud Seat Easy Charge WMM003N/Wireless Music Router WPR001N) dedicated, baud rate 115200, reset button GPIO#12
breed-ar9331-wr710n.bin	TP-LINK WR710N/WR720N v3 dedicated, baud rate 115200, reset button GPIO#11
breed-ar9331-hiwifi-hc6361.bin	Dedicated to Ji Router Jiyi (HC6361), only supports TP  firmware , baud rate 115200, reset button GPIO#11
breed-ar9341.bin	AR9341 general purpose, baud rate 115200, reset button GPIO#17
breed-ar9341-wnr2000v4.bin	Netgear WNR2000 v4 dedicated, baud rate 115200, reset button GPIO#4
breed-ar9341-pisen-wmp002n.bin	PISEN Cloud TV series watching WMP002N dedicated, baud rate 115200, reset button GPIO#17
breed-ar9341-wr800n.bin	TP-LINK WR800N dedicated, baud rate 115200, reset button GPIO#18
breed-ar9342-wr1041nv2.bin	TP-LINK WR1042N v2 dedicated, baud rate 115200, reset button GPIO#14
breed-ar9342-huawei-ws322.bin	Dedicated for Huawei WS322, baud rate 115200, reset key GPIO#0, WPS key GPIO#16
breed-ar9344.bin	AR9344 100M version, general purpose, baud rate 115200, reset button GPIO#16
breed-ar9344-ar8327n.bin	AR9344 + AR8327N Gigabit version, general purpose, baud rate 115200, reset button GPIO#16
breed-ar9344-wdr3320v2.bin	TP-LINK WDR3320 v2 dedicated, baud rate 115200, reset button GPIO#16
breed-ar9344-wr941nv6.bin	TP-LINK WR941N v6 dedicated, baud rate 115200, reset button GPIO#12
breed-ar9344-mw4530r.bin	Mercury MW4530R dedicated, baud rate 115200, reset key GPIO#17, QSS key GPIO#16
breed-ar9344-wndr4300-nand.bin	Netgear WNDR4300/WNDR3700 v4 dedicated, NAND boot, baud rate 115200, reset key GPIO#21, QSS key GPIO#12
breed-ar9344-wndr4300-spi.bin	Netgear WNDR4300/WNDR3700 v4 dedicated, SPI boot, baud rate 115200, reset key GPIO#21, QSS key GPIO#12
breed-ar9344-wndr4300-spi-recovery.bin	Netgear WNDR4300/WNDR3700 v4 dedicated, SPI boot, only for recovery purposes, baud rate 115200, reset key GPIO#21, QSS key GPIO#12
breed-ar9344-belair20e11.bin	BelAir20E-11 dedicated, baud rate 115200, reset key GPIO#17, WPS key GPIO#12
breed-ar9344-sgr-w500-n85b-v2.bin	GRENTECH SGR-W500-N85b v2 dedicated, baud rate 115200, support RTL8211E, reset button GPIO#3
breed-qca953x.bin	QCA9531/QCA9533, general purpose, baud rate 115200, reset key GPIO#12
breed-qca953x-letv-lba-047-ch.bin	Dedicated for LeTV router, baud rate 115200, reset button GPIO#17
breed-qca9558-wr941nv7.bin	TP-LINK WR941N v7 dedicated, baud rate 115200, reset button GPIO#17
breed-qca9558-ar8236.bin	QCA9558 + AR8236 100M version, general purpose, baud rate 115200, reset button GPIO#16
breed-qca9558-ar8327n.bin	QCA9558 + AR8327N Gigabit version, general purpose, baud rate 115200, reset button GPIO#16
breed-qca9558-wr2041nv2.bin	TP-LINK WR2041N v2 dedicated, baud rate 115200, reset button GPIO#17
breed-qca9558-wr1043ndv2.bin	TP-LINK WR1043ND v2 dedicated, baud rate 115200, reset button GPIO#16
breed-qca9558-dw33d.bin	Dedicated for Damai DW33D, baud rate 115200, reset button GPIO#17
breed-qca956x-uart_rx18_tx20-reset1.bin	QCA956X Universal, 100M/1000M adaptive, baud rate 115200, UART RX GPIO#18, TX GPIO#20, reset button GPIO#1
breed-qca956x-uart_rx18_tx20-reset2.bin	QCA956X Universal, 100M/1000M adaptive, baud rate 115200, UART RX GPIO#18, TX GPIO#20, reset button GPIO#2
breed-qca956x-uart_rx18_tx22-reset1.bin	QCA956X Universal, 100M/1000M adaptive, baud rate 115200, UART RX GPIO#18, TX GPIO#22, reset button GPIO#1
breed-qca956x-uart_rx18_tx22-reset2.bin	QCA956X Universal, 100M/1000M adaptive, baud rate 115200, UART RX GPIO#18, TX GPIO#22, reset button GPIO#2
breed-qca956x-uart_rx19_tx20-reset1.bin	QCA956X Universal, 100M/1000M adaptive, baud rate 115200, UART RX GPIO#19, TX GPIO#20, reset button GPIO#1
breed-qca956x-uart_rx19_tx20-reset2.bin	QCA956X Universal, 100M/1000M adaptive, baud rate 115200, UART RX GPIO#19, TX GPIO#20, reset button GPIO#2
breed-qca956x-uart_rx19_tx20-reset1.bin	QCA956X Universal, 100M/1000M adaptive, baud rate 115200, UART RX GPIO#19, TX GPIO#22, reset button GPIO#1
breed-qca956x-uart_rx19_tx22-reset2.bin	QCA956X Universal, 100M/1000M adaptive, baud rate 115200, UART RX GPIO#19, TX GPIO#22, reset button GPIO#2
breed-qca956x-uart_rx20_tx22-reset1.bin	QCA956X Universal, 100M/1000M adaptive, baud rate 115200, UART RX GPIO#20, TX GPIO#22, reset button GPIO#1
breed-qca956x-uart_rx20_tx22-reset2.bin	QCA956X Universal, 100M/1000M adaptive, baud rate 115200, UART RX GPIO#20, TX GPIO#22, reset button GPIO#2
breed-qca956x-reset2.bin	QCA956X 100M version, general purpose, baud rate 115200, reset button GPIO#2
breed-qca9561-wdr6500v2.bin (no longer updated)	TP-LINK WDR6500 v2 dedicated, baud rate 115200, reset button GPIO#1
breed-qca9563-wndr4500v3.bin	Netgear WNDR4500 v3 dedicated, baud rate 115200, reset button GPIO#2, WPS button GPIO#1
breed-qca9563-phicomm-k2t.bin	Phicomm K2T dedicated, baud rate 115200, reset button GPIO#2
breed-qca9563-rosinson-wr818.bin	Dedicated for ROSINSON WR818, baud rate 115200, reset button GPIO#2
breed-qca9563-jhr-848q.bin	JHR-848Q dedicated, baud rate 115200, reset button GPIO#2
breed-qca9563-dir-859-a.bin	D-Link DIR-859 A1/A2 dedicated, baud rate 115200, reset button GPIO#2
breed-tp9343.bin	TP9343, general purpose, baud rate 115200, reset key GPIO#1, WPS key GPIO#1

Note: The special version can light up all LEDs.

The following is a special version that supports custom reset button GPIO
file name	illustrate
breed-ar7161-blank.bin	AR7161 dedicated, supports AR8035 IP1001 MV88E1116 BCM5481 Gigabit PHY
breed-ar913x-blank.bin	AR913X only supports 88E6060 100M switch
breed-ar724x-blank.bin	AR724X dedicated, supports built-in 100M switch and AR8021 Gigabit PHY
breed-ar9331-blank.bin	AR9331 only supports built-in 100M switch
breed-ar934x-blank.bin	Dedicated to AR934X, supports built-in 100M switch and AR8327(N) Gigabit switch, AR8035 RTL8211E Gigabit PHY, RTL8201 100M PHY
breed-mt7620-blank.bin	Dedicated to MT7620, only supports built-in 100M switch
breed-mt76x8-blank.bin	Dedicated to MT7628/MT7688, only supports built-in 100M switch
breed-rt305x-nor-blank.bin	RT305X dedicated, boot from NOR flash memory, only supports built-in 100M switch
breed-rt305x-spi-blank.bin	RT305X dedicated, boot from SPI flash memory, only supports built-in 100M switch
breed-rt5350-blank.bin	RT5350 only supports built-in 100M switch
