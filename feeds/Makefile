include $(TOPDIR)/rules.mk

PKG_NAME:=example

PKG_VERSION:=0.0.1
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package-version-override.mk
include $(INCLUDE_DIR)/package.mk

# use SPACES here instead of tabs
define Package/example
  CATEGORY:=Sample
  SUBMENU:=Apps
  TITLE:=Example
  DEPENDS:=+libpcap +librt +libevent2-core 
endef

define Package/example/description
An example utility
endef

define Package/example/install
        $(INSTALL_DIR) $(1)/etc
        $(INSTALL_BIN) ./files/config $(1)/etc
endef

# NO TABS, NO SPACES
$(eval $(call BuildPackage,example))
