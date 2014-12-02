include $(TOPDIR)/rules.mk

PKG_NAME:=hworld
PKG_SOURCE_PROTO:=git
PKG_VERSION:=0.0.1
PKG_RELEASE:=1
PKG_SOURCE_URL:=https://github.com/ethanmorris/ExampleSource
PKG_BRANCH:=master
PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.gz
PKG_SOURCE_VERSION:=59a044b2d67ec44aac78485a9a5a145ca14714f8
PKG_SOURCE_SUBDIR:=$(PKG_NAME)-$(PKG_VERSION)

include $(INCLUDE_DIR)/package-version-override.mk
include $(INCLUDE_DIR)/package.mk

# use SPACES here instead of tabs
define Package/hworld
  CATEGORY:=Sample
  SUBMENU:=Apps
  TITLE:=Hello World
endef

define Package/hworld/description
An example program
endef

define Package/hworld/install
	$(INSTALL_DIR) $(1)/etc/hworld
	$(INSTALL_BIN) ./files/config $(1)/etc/hworld
	$(INSTALL_DIR) $(1)/usr/bin/
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/hworld $(1)/usr/bin/
endef

# NO TABS, NO SPACES
$(eval $(call BuildPackage,hworld))
