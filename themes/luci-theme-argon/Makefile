#
# Copyright (C) 2008-2019 Jerrykuku
#
# This is free software, licensed under the Apache License, Version 2.0 .
#

include $(TOPDIR)/rules.mk
TARGET_CFLAGS += -O3 -pipe -funroll-loops -march=armv8-a+crypto+crc -mcpu=cortex-a53+crypto+crc -mtune=cortex-a53

LUCI_TITLE:=Argon Theme
LUCI_DEPENDS:=+wget +jsonfilter

CONFIG_LUCI_CSSTIDY:=

define Package/luci-theme-argon/conffiles
/www/luci-static/argon/background/
endef

include ../../luci.mk

# call BuildPackage - OpenWrt buildroot signature
