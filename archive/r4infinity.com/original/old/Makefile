.PHONY: package

export TOPDIR := $(CURDIR)
export BASE   := r4infinity.com/original/$(shell basename $(CURDIR))
export OUT    := $(TOPDIR)/../../../../out
export COMMON := $(TOPDIR)/../../../../common-kernels

package: directory r4infinity.com_original_Kernel_2.1.zip

directory:
	mkdir -p $(OUT)/$(BASE)

r4infinity.com_original_Kernel_2.1.zip: directory
	cd $(TOPDIR)/r4infinity.com_original_Kernel_2.1 && zip -r $(OUT)/$(BASE)/$@ *
