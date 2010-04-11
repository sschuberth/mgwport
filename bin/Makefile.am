nodist_bin_SCRIPTS = mgwport
nodist_noinst_SCRIPTS = mgwport-inplace

mgwport: mgwport.in $(top_srcdir)/configure Makefile
	$(AM_V_GEN)sed	-e "s!\@VERSION\@!$(VERSION)!"			\
		-e "s!\@mgwclassdir\@!$(pkgdatadir)/mgwclass!"	\
		-e "s!\@docdir\@!$(docdir)!"			\
		-e "s!\@gnuconfigdir\@!$(pkgdatadir)!"		\
		-e "s!\@pkgdatadir\@!$(pkgdatadir)!"	\
		-e "s!\@pkglibdir\@!$(pkglibdir)!"		\
		-e "s!\@sysconfdir\@!$(sysconfdir)!"	\
		$< > $@ ; \
	chmod 755 $@

mgwport-inplace: mgwport.in $(top_srcdir)/configure Makefile
	$(AM_V_GEN)sed	-e "s!\@VERSION\@!$(VERSION)!"			\
		-e "s!\@mgwclassdir\@!$(abs_top_srcdir)/mgwclass!"	\
		-e "s!\@docdir\@!$(docdir)!"			\
		-e "s!\@gnuconfigdir\@!$(abs_top_srcdir)/data/gnuconfig!"		\
		-e "s!\@pkgdatadir\@!$(abs_top_srcdir)/data!"		\
		-e "s!\@pkglibdir\@!$(abs_top_srcdir)/lib!"			\
		-e "s!\@sysconfdir\@!$(abs_top_srcdir)/data!"		\
		$< > $@ ; \
	chmod 755 $@

EXTRA_DIST = mgwport.in
CLEANFILES = mgwport mgwport-inplace
