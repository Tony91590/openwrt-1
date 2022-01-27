include $(TOPDIR)/rules.mk

ARCH:=aarch64
BOARD:=ipq807x
BOARDNAME:=Qualcomm IPQ807x
FEATURES:=squashfs ramdisk fpu nand source-only
KERNELNAME:=Image dtbs
CPU_TYPE:=cortex-a53
SUBTARGETS:=generic

KERNEL_PATCHVER:=5.10

include $(INCLUDE_DIR)/target.mk
DEFAULT_PACKAGES += \
	kmod-usb3 kmod-usb-dwc3 kmod-usb-dwc3-qcom \
	kmod-leds-gpio kmod-gpio-button-hotplug \
	ath11k-firmware-ipq8074 kmod-ath11k-ahb \
	kmod-qca-nss-dp kmod-qca-nss-drv kmod-qca-nss-drv-pppoe kmod-qca-nss-ecm kmod-qca-nss-drv-bridge-mgr nss-firmware-ipq8074 \
	wpad-basic-wolfssl 

$(eval $(call BuildTarget))
