# SPDX-License-Identifier: Apache-2.0
#
# Copyright (C) 2023 ImmortalWrt.org

include $(TOPDIR)/rules.mk
TARGET_CFLAGS += -Os -pipe -funroll-loops -march=armv8-a+crypto+crc -mcpu=cortex-a53+crypto+crc -mtune=cortex-a53
TARGET_LDFLAGS += -Wl,-O2

LUCI_TITLE:=LuCI app for dae dashboard
LUCI_DEPENDS:=+daed +daed-geoip +daed-geosite
LUCI_PKGARCH:=all

include ../../luci.mk

# call BuildPackage - OpenWrt buildroot signature
