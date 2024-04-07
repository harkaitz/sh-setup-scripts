PROJECT=sh-setup-scripts
VERSION=1.0.0
PREFIX=/usr/local
all:
clean:
install:

## -- BLOCK:license --
install: install-license
install-license: 
	mkdir -p $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
	cp LICENSE $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
## -- BLOCK:license --
## -- BLOCK:sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/sbin
        if ($(shell uname -s),Windows_NT)
	  cp w/wsetup-git       $(DESTDIR)$(PREFIX)/sbin
	  cp w/wsetup-power     $(DESTDIR)$(PREFIX)/sbin
	  cp w/wsetup-prefix    $(DESTDIR)$(PREFIX)/sbin
	  cp w/wsetup-python312 $(DESTDIR)$(PREFIX)/sbin
	  cp w/wsetup-consoleZ  $(DESTDIR)$(PREFIX)/sbin
        endif
## -- BLOCK:sh --
