include $(TOPDIR)/rules.mk

PKG_NAME:=ntfs3-oot-mount
PKG_RELEASE:=2

include $(INCLUDE_DIR)/package.mk

define Package/ntfs3-oot-mount
	SECTION:=utils
	CATEGORY:=Utilities
	SUBMENU:=Filesystem
	TITLE:=NTFS mount script for Paragon NTFS3 driver
	PKGARCH:=all
	DEPENDS:=+kmod-fs-ntfs3-oot
endef

define Build/Configure
endef

define Build/Compile
endef

define Package/ntfs3-oot-mount/install
	$(INSTALL_DIR) $(1)/sbin
	$(INSTALL_BIN) ./files/mount.ntfs3 $(1)/sbin
endef

$(eval $(call BuildPackage,ntfs3-oot-mount))
