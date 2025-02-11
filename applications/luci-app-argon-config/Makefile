include $(TOPDIR)/rules.mk
TARGET_CFLAGS += -Os -pipe -funroll-loops -march=armv8-a+crypto+crc -mcpu=cortex-a53+crypto+crc -mtune=cortex-a53
TARGET_LDFLAGS += -Wl,-O2

LUCI_TITLE:=LuCI for Argon theme configuration
LUCI_PKGARCH:=all
LUCI_DEPENDS:=+luci-theme-argon

include ../../luci.mk

# call BuildPackage - OpenWrt buildroot signature
