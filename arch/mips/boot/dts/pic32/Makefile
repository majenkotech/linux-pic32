dtb-$(CONFIG_DTB_PIC32_MZDA_SK)		+= pic32mzda_sk.dtb
dtb-$(CONFIG_DTB_PIC32_MZDA_EVK)		+= pic32mzda_evk.dtb

dtb-$(CONFIG_DTB_PIC32_NONE)		+= \
					pic32mzda_sk.dtb \
					pic32mzda_evk.dtb

obj-y				+= $(patsubst %.dtb, %.dtb.o, $(dtb-y))

# Force kbuild to make empty built-in.o if necessary
obj-				+= dummy.o

always				:= $(dtb-y)
clean-files			:= *.dtb *.dtb.S
