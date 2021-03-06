#
# Copyright (C) 2006-2014 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=flyscripts
PKG_VERSION:=2.0.1
PKG_RELEASE:=1
PKG_LICENSE:=GPL-2.0

include $(INCLUDE_DIR)/package.mk

define Package/flyscripts/default
  SECTION:=base
  CATEGORY:=Extra packages
  DEPENDS:=+comgt
  MAINTAINER:=Zig Fisher <flyrouter@gmail.com>
  TITLE:=Base FlyRouter scripts
  URL:=https://github.com/ZigFisher/Glutinium/tree/master/flyscripts
endef

define Package/flyscripts_base
$(call Package/flyscripts/default)
  TITLE:=Base FlyRouter scripts
endef

define Package/flyscripts_octonix_bricket_base
$(call Package/flyscripts/default)
  TITLE:=Custom project settings
endef

define Package/flyscripts_octonix_bricket_msl
$(call Package/flyscripts/default)
  TITLE:=Custom project settings
endef

define Package/flyscripts_octonix_bricket_ukrn
$(call Package/flyscripts/default)
  TITLE:=Custom project settings
endef

define Package/flyscripts_rkeeper_wr841n_base
$(call Package/flyscripts/default)
  TITLE:=Custom project settings
endef

define Package/flyscripts_crmifc_wr841n_tuneller
$(call Package/flyscripts/default)
  TITLE:=Custom project settings
endef

define Package/flyscripts_switron_rt2257_base
$(call Package/flyscripts/default)
  TITLE:=Custom project settings
endef

define Package/flyscripts_zftlab_bricket_base
$(call Package/flyscripts/default)
  TITLE:=Custom project settings
endef

define Package/flyscripts_zftlab_bricket_flypeek
$(call Package/flyscripts/default)
  TITLE:=Custom project settings
endef

define Package/flyscripts_zftlab_bricket_mywifi
$(call Package/flyscripts/default)
  TITLE:=Custom project settings
endef

define Build/Configure
endef

define Build/Compile
endef

define Package/flyscripts_base/install
	$(INSTALL_DIR)  $(1)/etc
	$(INSTALL_BIN)  ./files/etc/rc.local.example $(1)/etc/
	$(INSTALL_BIN)  ./files/etc/ser2net.conf $(1)/etc/
	$(INSTALL_DIR)  $(1)/etc/config
	$(INSTALL_BIN)  ./files/etc/config/snmpd $(1)/etc/config/
	$(INSTALL_DIR)  $(1)/etc/hotplug.d/iface
	$(INSTALL_BIN)  ./files/etc/hotplug.d/iface/10-indicator $(1)/etc/hotplug.d/iface/
	$(INSTALL_BIN)  ./files/etc/hotplug.d/iface/12-vtun $(1)/etc/hotplug.d/iface/
	$(INSTALL_BIN)  ./files/etc/hotplug.d/iface/15-vtun $(1)/etc/hotplug.d/iface/
	$(INSTALL_DIR)  $(1)/etc/hotplug.d/usb
	$(INSTALL_BIN)  ./files/etc/hotplug.d/usb/30-com-* $(1)/etc/hotplug.d/usb/
	$(INSTALL_BIN)  ./files/etc/hotplug.d/usb/30-gps-* $(1)/etc/hotplug.d/usb/
	$(INSTALL_BIN)  ./files/etc/hotplug.d/usb/30-modem-* $(1)/etc/hotplug.d/usb/
	$(INSTALL_BIN)  ./files/etc/hotplug.d/usb/30-rs485-* $(1)/etc/hotplug.d/usb/
	$(INSTALL_DIR)  $(1)/lib/netifd/proto
	$(INSTALL_BIN)  ./files/lib/netifd/proto/3g.sh $(1)/lib/netifd/proto/
	$(INSTALL_BIN)  ./files/lib/netifd/proto/vtun.sh $(1)/lib/netifd/proto/
	$(INSTALL_DIR)  $(1)/usr/sbin
	$(INSTALL_BIN)  ./files/usr/sbin/license.sh $(1)/usr/sbin/
endef

define Package/flyscripts_octonix_bricket_base/install
	$(INSTALL_DIR)  $(1)/etc
	$(INSTALL_BIN)  ./files/etc/banner__octonix_bricket_base $(1)/etc/banner
	$(INSTALL_DIR)  $(1)/etc/uci-defaults
	$(INSTALL_BIN)  ./files/etc/uci-defaults/55_octonix_bricket_base $(1)/etc/uci-defaults/
endef

define Package/flyscripts_octonix_bricket_msl/install
	$(INSTALL_DIR)  $(1)/etc
	$(INSTALL_BIN)  ./files/etc/banner__octonix_bricket_msl $(1)/etc/banner
	$(INSTALL_DIR)  $(1)/etc/uci-defaults
	$(INSTALL_BIN)  ./files/etc/uci-defaults/55_octonix_bricket_msl $(1)/etc/uci-defaults/
endef

define Package/flyscripts_octonix_bricket_ukrn/install
	$(INSTALL_DIR)  $(1)/etc
	$(INSTALL_BIN)  ./files/etc/banner__octonix_bricket_ukrn $(1)/etc/banner
	$(INSTALL_DIR)  $(1)/etc/uci-defaults
	$(INSTALL_BIN)  ./files/etc/uci-defaults/55_octonix_bricket_ukrn $(1)/etc/uci-defaults/
endef

define Package/flyscripts_rkeeper_wr841n_base/install
	$(INSTALL_DIR)  $(1)/etc
	$(INSTALL_BIN)  ./files/etc/banner__rkeeper_wr841n_base $(1)/etc/banner
	$(INSTALL_DIR)  $(1)/etc/uci-defaults
	$(INSTALL_BIN)  ./files/etc/uci-defaults/55_rkeeper_wr841n_base $(1)/etc/uci-defaults/
endef

define Package/flyscripts_crmifc_wr841n_tuneller/install
	$(INSTALL_DIR)  $(1)/etc
	$(INSTALL_BIN)  ./files/etc/banner__crmifc_wr841n_tuneller $(1)/etc/banner
	$(INSTALL_DIR)  $(1)/etc/uci-defaults
	$(INSTALL_BIN)  ./files/etc/uci-defaults/55_crmifc_wr841n_tuneller $(1)/etc/uci-defaults/
endef

define Package/flyscripts_switron_rt2257_base/install
	$(INSTALL_DIR)  $(1)/etc
	$(INSTALL_BIN)  ./files/etc/banner__switron_rt2257_base $(1)/etc/banner
	$(INSTALL_DIR)  $(1)/etc/uci-defaults
	$(INSTALL_BIN)  ./files/etc/uci-defaults/55_switron_rt2257_base $(1)/etc/uci-defaults/
endef

define Package/flyscripts_zftlab_bricket_base/install
	$(INSTALL_DIR)  $(1)/etc
	$(INSTALL_BIN)  ./files/etc/banner__zftlab_bricket_base $(1)/etc/banner
	$(INSTALL_DIR)  $(1)/etc/uci-defaults
	$(INSTALL_BIN)  ./files/etc/uci-defaults/55_zftlab_bricket_base $(1)/etc/uci-defaults/
	$(INSTALL_DIR)  $(1)/etc/hotplug.d/net
	$(INSTALL_BIN)  ./files/etc/hotplug.d/net/37-vtun $(1)/etc/hotplug.d/net/
	$(INSTALL_DIR)  $(1)/etc/hotplug.d/usb
	$(INSTALL_BIN)  ./files/etc/hotplug.d/usb/30-logger $(1)/etc/hotplug.d/usb/
endef

define Package/flyscripts_zftlab_bricket_flypeek/install
	$(INSTALL_DIR)  $(1)/etc
	$(INSTALL_BIN)  ./files/etc/banner__zftlab_bricket_flypeek $(1)/etc/banner
	$(INSTALL_DIR)  $(1)/etc/uci-defaults
	$(INSTALL_BIN)  ./files/etc/uci-defaults/55_zftlab_bricket_flypeek $(1)/etc/uci-defaults/
	$(INSTALL_DIR)  $(1)/usr/sbin
	$(INSTALL_BIN)  ./files/usr/sbin/service_flypeek_usb_yandex.sh $(1)/usr/sbin/
	$(INSTALL_BIN)  ./files/usr/sbin/service_flypeek_usb.sh $(1)/usr/sbin/
	$(INSTALL_BIN)  ./files/usr/sbin/service_flypeek_ipc.sh $(1)/usr/sbin/
endef

define Package/flyscripts_zftlab_bricket_mywifi/install
	$(INSTALL_DIR)  $(1)/etc
	$(INSTALL_BIN)  ./files/etc/banner__zftlab_bricket_mywifi $(1)/etc/banner
	$(INSTALL_DIR)  $(1)/etc/uci-defaults
	$(INSTALL_BIN)  ./files/etc/uci-defaults/55_zftlab_bricket_mywifi $(1)/etc/uci-defaults/
endef


$(eval $(call BuildPackage,flyscripts_base))
$(eval $(call BuildPackage,flyscripts_octonix_bricket_base))
$(eval $(call BuildPackage,flyscripts_octonix_bricket_msl))
$(eval $(call BuildPackage,flyscripts_octonix_bricket_ukrn))
$(eval $(call BuildPackage,flyscripts_rkeeper_wr841n_base))
$(eval $(call BuildPackage,flyscripts_crmifc_wr841n_tuneller))
$(eval $(call BuildPackage,flyscripts_switron_rt2257_base))
$(eval $(call BuildPackage,flyscripts_zftlab_bricket_base))
$(eval $(call BuildPackage,flyscripts_zftlab_bricket_flypeek))
$(eval $(call BuildPackage,flyscripts_zftlab_bricket_mywifi))
