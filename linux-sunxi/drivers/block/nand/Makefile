
################################################################################
#
# Common Variables that already set:
#     LICHEE_KDIR
#     LICHEE_MOD_DIR
#     CROSS_COMPILE
#     ARCH
#
#################################################################################
PWD=$(shell pwd)
			 
ifneq ($(strip $(CONFIG_ARCH_SUN8IW1P1)),)
obj-y += sun8iw1p1/
endif

ifneq ($(strip $(CONFIG_ARCH_SUN8IW3P1)),)
obj-y += sun8iw3p1/
endif

ifneq ($(strip $(CONFIG_ARCH_SUN9IW1P1)),)
obj-y += sun9iw1p1/
endif

ifneq ($(strip $(CONFIG_ARCH_SUN8IW5P1)),)
obj-y += sun8iw5p1/
endif

ifneq ($(strip $(CONFIG_ARCH_SUN8IW6P1)),)
obj-y += sun8iw6p1/
endif

ifneq ($(strip $(CONFIG_ARCH_SUN8IW7P1)),)
obj-y += sun8iw7p1/
endif

ifneq ($(strip $(CONFIG_ARCH_SUN8IW9P1)),)
obj-y += sun8iw9p1/
endif


ifneq ($(strip $(CONFIG_ARCH_SUN50IW1P1)),)
obj-y += sun50iw1p1/
endif

ifneq ($(strip $(CONFIG_ARCH_SUN8IW10P1)),)
obj-y += sun8iw10p1/
endif

ifneq ($(strip $(CONFIG_ARCH_SUN8IW11P1)),)
obj-y += sun8iw11p1/
endif

ifneq ($(strip $(CONFIG_ARCH_SUN50IW2P1)),)
obj-y += sun50iw2p1/
endif

install: build	
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW1P1=y" >/dev/null 2>&1;then \
	cp sun8iw1p1/nand.ko $(LICHEE_MOD_DIR)/;\
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW3P1=y" >/dev/null 2>&1;then \
	cp sun8iw3p1/nand.ko $(LICHEE_MOD_DIR)/;\
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN9IW1P1=y" >/dev/null 2>&1;then \
	cp sun9iw1p1/nand.ko $(LICHEE_MOD_DIR)/;\
	fi 
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW5P1=y" >/dev/null 2>&1;then \
	cp sun8iw5p1/nand.ko $(LICHEE_MOD_DIR)/;\
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW6P1=y" >/dev/null 2>&1;then \
	cp sun8iw6p1/nand.ko $(LICHEE_MOD_DIR)/;\
	fi	 
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW7P1=y" >/dev/null 2>&1;then \
	cp sun8iw7p1/nand.ko $(LICHEE_MOD_DIR)/;\
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW9P1=y" >/dev/null 2>&1;then \
	cp sun8iw9p1/nand.ko $(LICHEE_MOD_DIR)/;\
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN50IW1P1=y" >/dev/null 2>&1;then \
	cp sun50iw1p1/nand.ko $(LICHEE_MOD_DIR)/;\
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW10P1=y" >/dev/null 2>&1;then \
	cp sun8iw10p1/nand.ko $(LICHEE_MOD_DIR)/;\
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW11P1=y" >/dev/null 2>&1;then \
	cp sun8iw11p1/nand.ko $(LICHEE_MOD_DIR)/;\
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN50IW2P1=y" >/dev/null 2>&1;then \
	cp sun50iw2p1/nand.ko $(LICHEE_MOD_DIR)/;\
	fi
	
build:
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW1P1=y" >/dev/null 2>&1;then \
	cp sun8iw1p1/libnand_sun8iw1p1 sun8iw1p1/libnand_sun8iw1p1.a;\
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW3P1=y" >/dev/null 2>&1;then \
	cp sun8iw3p1/libnand_sun8iw3p1 sun8iw3p1/libnand_sun8iw3p1.a;\
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN9IW1P1=y" >/dev/null 2>&1;then \
	cp sun9iw1p1/libnand_sun9iw1p1 sun9iw1p1/libnand_sun9iw1p1.a;\
	fi	
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW5P1=y" >/dev/null 2>&1;then \
	cp sun8iw5p1/libnand_sun8iw5p1 sun8iw5p1/libnand_sun8iw5p1.a;\
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW6P1=y" >/dev/null 2>&1;then \
	cp sun8iw6p1/libnand_sun8iw6p1 sun8iw6p1/libnand_sun8iw6p1.a;\
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW7P1=y" >/dev/null 2>&1;then \
	cp sun8iw7p1/libnand_sun8iw7p1 sun8iw7p1/libnand_sun8iw7p1.a;\
	fi	
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW9P1=y" >/dev/null 2>&1;then \
	cp sun8iw9p1/libnand_sun8iw9p1 sun8iw9p1/libnand_sun8iw9p1.a;\
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN50IW1P1=y" >/dev/null 2>&1;then \
	if cat ../../.config|grep "CONFIG_ARM64=y" >/dev/null 2>&1;then \
	cp sun50iw1p1/libnand_sun50iw1p1 sun50iw1p1/libnand_sun50iw1p1.a;\
	else \
	cp sun50iw1p1/libnand_sun50iw1p1_32 sun50iw1p1/libnand_sun50iw1p1.a;\
	fi \
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW10P1=y" >/dev/null 2>&1;then \
	cp sun8iw10p1/libnand_sun8iw10p1 sun8iw10p1/libnand_sun8iw10p1.a;\
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN8IW11P1=y" >/dev/null 2>&1;then \
	cp sun8iw11p1/libnand_sun8iw11p1 sun8iw11p1/libnand_sun8iw11p1.a;\
	fi
	@if cat ../../.config|grep "CONFIG_ARCH_SUN50IW2P1=y" >/dev/null 2>&1;then \
	cp sun50iw2p1/libnand_sun50iw2p1 sun50iw2p1/libnand_sun50iw2p1.a;\
	fi
	$(MAKE) -C $(LICHEE_KDIR) M=$(PWD)

clean:
	@rm -rf *.o *.ko .*.cmd *.mod.c *.order *.symvers .tmp_versions *~
