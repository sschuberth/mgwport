doc_DATA =

if HAVE_HELP2MAN

man_MANS = mgwport.1

mgwport.1: $(top_builddir)/bin/mgwport-inplace $(top_srcdir)/lib/help.mgwpart
	$(AM_V_GEN)$(HELP2MAN) -o $@ --no-info --name="MinGW/MSYS source packaging tool" $<

if HAVE_GROFF

doc_DATA += mgwport.1.html

mgwport.1.html: mgwport.1
	$(AM_V_GEN)$(GROFF) -t -mandoc -Thtml $< > $@

endif HAVE_GROFF
endif HAVE_HELP2MAN

if HAVE_ROBODOC

doc_DATA += manual.html manual.css

manual.html: $(srcdir)/robodoc.rc $(wildcard $(top_srcdir)/mgwclass/*.mgwclass) $(wildcard $(top_srcdir)/lib/*.mgwpart) $(top_srcdir)/bin/mgwport.in $(wildcard $(top_srcdir)/data/*)
	$(AM_V_GEN)cd $(top_srcdir) && $(ROBODOC) --src . --doc $(abs_builddir)/manual --rc $(abs_srcdir)/robodoc.rc --html --singledoc

manual.css: manual.html

endif HAVE_ROBODOC

CLEANFILES = $(man_MANS) $(doc_DATA)

EXTRA_DIST = robodoc.rc
