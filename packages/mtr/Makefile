#
# Copyright (C) 2011-2014 Entware
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

all: .done

.done:
	patch -d $(TOP) -p3 -i $(CURDIR)/fix-path.patch
	cp -f ./600-libresolv.patch ../../../openwrt_trunk/feeds/packages/net/mtr/patches/
	@touch $@

clean:
	@rm -f .done

.PHONY: clean
