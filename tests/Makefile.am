TESTS = messages bootstrap

TESTS_ENVIRONMENT = MAKE=$(MAKE) PACKAGE=$(PACKAGE) VERSION=$(VERSION) top_srcdir=$(top_srcdir) top_builddir=$(top_builddir)

EXTRA_DIST = $(TESTS)

CLEANFILES = \
	foo-1.2.3-4.mgwport \
	$(PACKAGE)-$(VERSION)-1-mingw32-src.tar.lzma \
	$(PACKAGE)-$(VERSION)-1-mingw32-bin.tar.lzma \
	$(PACKAGE)-$(VERSION)-1-mingw32-doc.tar.lzma \
	$(PACKAGE)-$(VERSION)-1-mingw32-lic.tar.lzma \
	$(PACKAGE)-$(VERSION)-1-msys-*-src.tar.lzma \
	$(PACKAGE)-$(VERSION)-1-msys-*-bin.tar.lzma \
	$(PACKAGE)-$(VERSION)-1-msys-*-doc.tar.lzma \
	$(PACKAGE)-$(VERSION)-1-msys-*-lic.tar.lzma \
	$(PACKAGE)-$(VERSION)-1.mgwport \
	$(PACKAGE)-$(VERSION)-1.msysport \
	$(PACKAGE)-$(VERSION).tar.xz

clean-local:
	-rm -fr $(PACKAGE)/ $(PACKAGE)-$(VERSION)-1/
