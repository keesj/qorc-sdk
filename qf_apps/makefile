BINS = qf_helloworldsw/GCC_Project/output/bin/qf_helloworldsw.bin\
	qf_helloworldhw/GCC_Project/output/bin/qf_helloworldhw.bin\
	qf_advancedfpga/GCC_Project/output/bin/qf_advancedfpga.bin\
	qf_bootloader/GCC_Project/output/bin/qf_bootloader.bin\
	qf_loadflash/GCC_Project/output/bin/qf_loadflash.bin\
	qf_mqttsn_ai_app/GCC_Project/output/bin/qf_mqttsn_ai_app.bin

MFGBINS = qf_bootloader/GCC_Project/output/bin/qf_bootloader.bin\
		qf_loadflash/GCC_Project/output/bin/qf_loadflash.bin\
		qf_helloworldsw/GCC_Project/output/bin/qf_helloworldsw.bin
all:	$(BINS)

clean:
	cd qf_helloworldsw/GCC_Project/ && make clean
	cd qf_helloworldhw/GCC_Project/ && make clean
	cd qf_advancedfpga/GCC_Project/ && make clean
	cd qf_bootloader/GCC_Project/ && make clean



qf_mfgpkg:	$(MFGBINS)
	cp $(MFGBINS) quickfeather-initial-binaries
	cp ../s3-gateware/usb2serial/usb2serial.bin quickfeather-initial-binaries/qf_bootfpga.bin


qf_helloworldsw/GCC_Project/output/bin/qf_helloworldsw.bin:
	cd qf_helloworldsw/GCC_Project/ && make

qf_helloworldhw/GCC_Project/output/bin/qf_helloworldhw.bin:
	cd qf_helloworldhw/GCC_Project/ && make

qf_advancedfpga/GCC_Project/output/bin/qf_advancedfpga.bin:
	cd qf_advancedfpga/GCC_Project/ && make

qf_bootloader/GCC_Project/output/bin/qf_bootloader.bin:
	cd qf_bootloader/GCC_Project/ && make
	
qf_loadflash/GCC_Project/output/bin/qf_loadflash.bin:
	cd qf_loadflash/GCC_Project/ && make

qf_mqttsn_ai_app/GCC_Project/output/bin/qf_mqttsn_ai_app.bin:
	cd qf_mqttsn_ai_app/GCC_Project/ && make
