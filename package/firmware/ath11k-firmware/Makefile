include $(TOPDIR)/rules.mk

PKG_NAME:=ath11k-firmware
PKG_VERSION:=19

PKG_MAINTAINER:=John Crispin <john@phrozen.org>

include $(INCLUDE_DIR)/package.mk

define Package/ath11k-firmware-default
  SECTION:=firmware
  CATEGORY:=Firmware
  URL:=$(PKG_SOURCE_URL)
  DEPENDS:=
endef

define Package/ath11k-firmware-ipq8074
$(Package/ath11k-firmware-default)
  TITLE:=ath11k firmware for IPQ8074 devices
endef

define Build/Compile

endef

define Package/ath11k-firmware-ipq8074/install
	$(INSTALL_DIR) $(1)/lib/firmware/IPQ8074/
	$(INSTALL_DATA) ./files/IPQ8074/* \
		$(1)/lib/firmware/IPQ8074/
endef

$(eval $(call BuildPackage,ath11k-firmware-ipq8074))
