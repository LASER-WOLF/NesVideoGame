##############################################################################
# Rule to assemble and link all assembly files
##############################################################################
all:
	ca65 loadbackground.asm -o loadbackground.o
	ld65 loadbackground.o   -o loadbackground.nes -C nes.cfg

##############################################################################
# Rule to remove all object (.o) and cartridge (.nes) files
##############################################################################
clean:
	rm *.o *.nes

##############################################################################
# Rule to run the final cartridge .nes file in the FCEUX emulator
##############################################################################
run:
	fceux loadbackground.nes
