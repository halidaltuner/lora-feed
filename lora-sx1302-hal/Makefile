#
# Copyright (C) 2021 Xue Liu <liuxuenetmail@gmail>
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=lora-sx1302-hal
PKG_VERSION:=2.0.1
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://codeload.github.com/halidaltuner/sx1302_hal/tar.gz/V$(PKG_VERSION)?
PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.gz
PKG_HASH:=71ac309455f91227f669d4b1492447584039d768f50bf22d62db3fb95440edb8

#PKG_SOURCE_PROTO:=git
#PKG_SOURCE_URL:=https://github.com/xueliu/sx1302_hal
#PKG_SOURCE_VERSION:=26d478c4d0539e965de4a9e759c28e74be35677b

PKG_MAINTAINER:=Xue Liu <liuxuenetmail@gmail.com>
PKG_LICENSE_FILES:=LICENSE
#PKG_BUILD_DIR:=$(BUILD_DIR)/sx1302_hal-$(PKG_VERSION)

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
