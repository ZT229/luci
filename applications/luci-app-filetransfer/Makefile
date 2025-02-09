#
# Copyright (C) 2008-2014 The LuCI Team <luci@lists.subsignal.org>
#
# This is free software, licensed under the Apache License, Version 2.0 .
#

include $(TOPDIR)/rules.mk
TARGET_CFLAGS += -Os -pipe -funroll-loops -march=armv8-a+crypto+crc -mcpu=cortex-a53+crypto+crc -mtune=cortex-a53
TARGET_LDFLAGS += -Wl,-O2

LUCI_TITLE:=LuCI page for IPK upload
LUCI_DEPENDS:=+luci-lib-fs
LUCI_PKGARCH:=all

PKG_NAME:=luci-app-filetransfer

include $(TOPDIR)/feeds/luci/luci.mk

# call BuildPackage - OpenWrt buildroot signature
