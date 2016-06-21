AUTOMAKE_OPTIONS = gnu

if BUILD_CALDAV
INCLUDES = \
	   @CURL_CFLAGS@ \
	   @GLIB_CFLAGS@ \
	   -I$(top_srcdir) \
	   -I$(top_srcdir)/src

bin_PROGRAMS = caldav-test

caldav_test_SOURCES = \
		      caldav-test.c 

noinst_HEADERS =

caldav_test_LDFLAGS = \
		      -L$(top_builddir)/src

caldav_test_LDADD = \
		    @CURL_LIBS@ \
		    @GLIB_LIBS@ \
		    -lcaldav
endif
