.PHONY: package

export TOPDIR := $(CURDIR)
export BASE   := $(shell basename $(CURDIR))
export OUT    := $(TOPDIR)/../../out
export COMMON := $(TOPDIR)/../../common-kernels

package: directory r4-new.com_Kernel_1.5.zip extdata

directory:
	mkdir -p $(OUT)/$(BASE)

r4-new.com_Kernel_1.5.zip: directory
	cd $(TOPDIR)/r4-new.com_Kernel_1.5 && zip -r $(OUT)/$(BASE)/$@ *

extdata: directory
	cp README.txt $(OUT)/$(BASE)
