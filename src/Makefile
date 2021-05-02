# Makefile for building BDSC using vcpm and enclosed LASM
export CPMDrive_D=$(PWD)
export CPMDefault=d:

all: cc.com cc2.com clink.com

cc2.com: cc2.asm cc2a.asm cc2b.asm cc2c.asm cc2d.asm cc2e.asm
	vcpm lasm cc2.ddd d:
	vcpm load cc2

cc.com:	cc.asm cca.asm ccb.asm ccc.asm ccd.asm
	vcpm lasm cc.ddd d:
	vcpm load cc

clink.com: clinkl.asm clinka.asm clinkb.asm
	vcpm lasm clinkl.ddd d:
	vcpm load clinkl
	mv clinkl.com $@
