dist_pkgdata_DATA = \
	mgwport.nanorc	\
	mirrors			\
	mono.snk		\
	sample.mgwport	\
	uac-manifest.in \
	autopoint.patch

dist_pkgdata_SCRIPTS =	\
	gnuconfig/config.guess		\
	gnuconfig/config.sub

mimedir = $(datadir)/mime/packages
dist_mime_DATA = mgwport.xml

bashcompletiondir = $(sysconfdir)/bash_completion.d
dist_bashcompletion_DATA = mgwport-bash-completion

install-data-local:
	if ! test -f $(DESTDIR)$(sysconfdir)/mgwport.conf ; then \
		$(mkinstalldirs) $(DESTDIR)$(sysconfdir) ; \
		$(INSTALL_DATA) $(srcdir)/mgwport.conf $(DESTDIR)$(sysconfdir) ; \
	fi

EXTRA_DIST = mgwport.conf
