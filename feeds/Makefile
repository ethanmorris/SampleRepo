include $(TOPDIR)/rules.mk

PKG_NAME:=hworld

PKG_VERSION:=0.0.1
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package-version-override.mk
include $(INCLUDE_DIR)/package.mk

# use SPACES here instead of tabs
define Package/hworld
  CATEGORY:=Sample
  SUBMENU:=Apps
  TITLE:=Hello World
  DEPENDS:=
endef

define Package/hworld/description
An example program
endef

define Package/hworld/install
        $(INSTALL_DIR) $(1)/etc
        $(INSTALL_BIN) ./files/config $(1)/etc
endef

# NO TABS, NO SPACES
$(eval $(call BuildPackage,hworld))
