include $(TOPDIR)/rules.mk

PKG_NAME:=student-db

PKG_VERSION:=1.0
PKG_RELEASE:=1
PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/vlicitis/student-db.git
PKG_SOURCE_VERSION:=main

PKG_MIRROR_HASH:=skip

PKG_MAINTAINER:=Viesturs Licitis <vllicitis@gmail.com>

include $(INCLUDE_DIR)/package.mk

define Package/student-db
	SECTION:=custom
	CATEGORY:=CUSTOM
	TITLE:=student-db
	DEPENDS:=+libc
endef

define Package/student-db/description
	Student DB - package for reading and writing database to file
endef

define Package/student-db/install
	$(INSTALL_DIR) $(1)/usr/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/student_db $(1)/usr/bin/
endef

$(eval $(call BuildPackage,student-db))

