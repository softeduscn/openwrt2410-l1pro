# Copyright (C) 2016 Openwrt.org
#
# This is free software, licensed under the Apache License, Version 2.0 .
#

include $(TOPDIR)/rules.mk

LUCI_TITLE:=LuCI support for VSFTPD
LUCI_DEPENDS:=+vsftpd
LUCI_PKGARCH:=all

PKG_NAME:=luci-app-vsftpd
PKG_VERSION:=1.0
PKG_RELEASE:=3

define Package/luci-app-vsftpd/install
	$(INSTALL_DIR) $(1)/usr/lib/lua/luci/i18n
	po2lmo ./po/zh_Hans/vsftpd.po $(1)/usr/lib/lua/luci/i18n/vsftpd.zh-cn.lmo
endef

include $(TOPDIR)/feeds/luci/luci.mk

# call BuildPackage - OpenWrt buildroot signature
