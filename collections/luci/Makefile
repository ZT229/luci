#
# Copyright (C) 2008-2014 The LuCI Team <luci@lists.subsignal.org>
#
# This is free software, licensed under the Apache License, Version 2.0 .
#

include $(TOPDIR)/rules.mk
TARGET_CFLAGS += -Os -pipe -funroll-loops -march=armv8-a+crypto+crc -mcpu=cortex-a53+crypto+crc -mtune=cortex-a53
TARGET_LDFLAGS += -Wl,-O2

LUCI_TYPE:=col
LUCI_BASENAME:=luci

LUCI_TITLE:=LuCI interface with Uhttpd as Webserver (default)
LUCI_DESCRIPTION:=Standard OpenWrt set including package management and attended sysupgrades support
LUCI_DEPENDS:= \
	+luci-light \
	+luci-app-package-manager

PKG_LICENSE:=Apache-2.0

include ../../luci.mk

# call BuildPackage - OpenWrt buildroot signature
