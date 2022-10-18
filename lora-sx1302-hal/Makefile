#
# Copyright (C) 2021 Xue Liu <liuxuenetmail@gmail>
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/halidaltuner/sx1302_hal
PKG_SOURCE_VERSION:=4b42025d1751e04632c0b04160e0d29dbbb222a5

PKG_MAINTAINER:=Xue Liu <liuxuenetmail@gmail.com>
PKG_LICENSE_FILES:=LICENSE

include $(INCLUDE_DIR)/package.mk
include $(INCLUDE_DIR)/cmake.mk

define Package/libsx1302
  SECTION:=libs
  CATEGORY:=Libraries
  TITLE:=Driver/HAL library for Semtech SX1302
  URL:=https://www.semtech.com/products/wireless-rf/lora-gateways/sx1302
  DEPENDS:=+kmod-spi-dev
endef


$(eval $(call BuildPackage,libsx1302))
