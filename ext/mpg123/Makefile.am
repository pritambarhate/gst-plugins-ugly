plugin_LTLIBRARIES = libgstmpg123.la

libgstmpg123_la_SOURCES = gstmpg123audiodec.c
libgstmpg123_la_CFLAGS = -DGST_USE_UNSTABLE_API \
	$(GST_PLUGINS_BASE_CFLAGS) \
	$(GST_BASE_CFLAGS) $(GST_CFLAGS) $(MPG123_CFLAGS)
libgstmpg123_la_LIBADD = $(GST_PLUGINS_BASE_LIBS) -lgstaudio-@GST_API_VERSION@ \
	$(GST_BASE_LIBS) $(GST_LIBS) $(MPG123_LIBS)
libgstmpg123_la_LDFLAGS = $(GST_PLUGIN_LDFLAGS)
libgstmpg123_la_LIBTOOLFLAGS = $(GST_PLUGIN_LIBTOOLFLAGS)

noinst_HEADERS = gstmpg123audiodec.h
