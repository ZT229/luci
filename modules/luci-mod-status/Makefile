#
# Copyright (C) 2008-2014 The LuCI Team <luci@lists.subsignal.org>
#
# This is free software, licensed under the Apache License, Version 2.0 .
#

include $(TOPDIR)/rules.mk
TARGET_CFLAGS += -Os -pipe -funroll-loops -march=armv8-a+crypto+crc -mcpu=cortex-a53+crypto+crc -mtune=cortex-a53
TARGET_LDFLAGS += -Wl,-O2

LUCI_TITLE:=LuCI Status Pages
LUCI_DEPENDS:=+luci-base +libiwinfo +rpcd-mod-iwinfo

PKG_RELEASE:=2
PKG_BUILD_DEPENDS:=iwinfo
PKG_LICENSE:=Apache-2.0

include ../../luci.mk

# call BuildPackage - OpenWrt buildroot signature

