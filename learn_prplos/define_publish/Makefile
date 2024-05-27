include $(TOPDIR)/rules.mk

PKG_NAME:=define-publish
PKG_VERSION:=1.0
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/define-publish
  SECTION:=prplos-learning
  CATEGORY:=Prplos Learning
  TITLE:=Prplos-Define-Publish!
endef

define Package/define-publish/description
  Define and Publish define-publish Example
endef

define Build/Prepare
		$(CP) -r labs $(PKG_BUILD_DIR)/
endef

define Build/Compile

endef

define Package/define-publish/install
		$(INSTALL_DIR) $(1)/etc/define_publish
		$(INSTALL_BIN) $(PKG_BUILD_DIR)/labs/lab1/* $(1)/etc/define_publish
		$(INSTALL_BIN) $(PKG_BUILD_DIR)/labs/lab2/* $(1)/etc/define_publish
endef

$(eval $(call BuildPackage,define-publish))