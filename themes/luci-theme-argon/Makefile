#
# Copyright (C) 2008-2019 Jerrykuku
#
# This is free software, licensed under the Apache License, Version 2.0 .
#

include $(TOPDIR)/rules.mk
TARGET_CFLAGS += -Os -pipe -funroll-loops -march=armv8-a+crypto+crc -mcpu=cortex-a53+crypto+crc -mtune=cortex-a53
TARGET_LDFLAGS += -Wl,-O2

LUCI_TITLE:=Argon Theme
LUCI_DEPENDS:=+wget +jsonfilter +luci-app-argon-config

PKG_VERSION:=2.3.2
PKG_RELEASE:=20250207

CONFIG_LUCI_CSSTIDY:=

define Package/luci-theme-argon/conffiles
/www/luci-static/argon/background/
endef

include ../../luci.mk

# call BuildPackage - OpenWrt buildroot signature
