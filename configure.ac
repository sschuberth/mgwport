AC_INIT(mgwport, 0.10.6,
	[mingw-users@lists.sourceforge.net])

AC_PREREQ([2.64])

AC_CONFIG_SRCDIR([bin/mgwport.in])

AM_INIT_AUTOMAKE([1.11 foreign dist-xz no-dist-gzip])

AM_MAINTAINER_MODE

m4_ifdef([AM_SILENT_RULES], [AM_SILENT_RULES([yes])])

AC_PATH_PROG(HELP2MAN, help2man)
AM_CONDITIONAL(HAVE_HELP2MAN, test "x$HELP2MAN" != "x")

AC_PATH_PROG(GROFF, groff)
AM_CONDITIONAL(HAVE_GROFF, test "x$GROFF" != "x")

AC_PATH_PROG(ROBODOC, robodoc)
AM_CONDITIONAL(HAVE_ROBODOC, test "x$ROBODOC" != "x")

AC_CONFIG_FILES([
Makefile
bin/Makefile
lib/Makefile
mgwclass/Makefile
data/Makefile
doc/Makefile
tests/Makefile
tools/Makefile
])

AC_OUTPUT
