TESTS = messages bootstrap

TESTS_ENVIRONMENT = MAKE=$(MAKE) PACKAGE=$(PACKAGE) VERSION=$(VERSION) top_srcdir=$(top_srcdir) top_builddir=$(top_builddir)

EXTRA_DIST = $(TESTS)

CLEANFILES = \
	foo-1.2.3-4.mgwport \
	$(PACKAGE)-$(VERSION)-1-src.tar.lzma \
	$(PACKAGE)-$(VERSION)-1.tar.lzma \
	$(PACKAGE)-$(VERSION)-1.mgwport \
	$(PACKAGE)-$(VERSION).tar.xz

clean-local:
	-rm -fr $(PACKAGE)/ $(PACKAGE)-$(VERSION)-1/
