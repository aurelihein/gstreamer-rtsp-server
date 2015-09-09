
bin_PROGRAMS = rtsp_server
rtsp_server_SOURCES = rtsp_server.c

AM_CPPFLAGS = @rtsp_server_CFLAGS@ @GSTREAMER_CFLAGS@ @GSTREAMERRTSP_CFLAGS@
AM_LDFLAGS = @rtsp_server_LIBS@ @GSTREAMER_LIBS@ @GSTREAMERRTSP_LIBS@ -lgstrtspserver-0.10

CLEANFILES = *~ 
