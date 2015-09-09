AC_PREREQ(2.61)

# package version number (not shared library version)
# odd micro numbers indicate in-progress development
# even micro numbers indicate released versions
m4_define(rtsp_server_version_major, 0)
m4_define(rtsp_server_version_minor, 1)
m4_define(rtsp_server_version_micro, 0)

m4_define([rtsp_server_version],
          [rtsp_server_version_major.rtsp_server_version_minor.rtsp_server_version_micro])
m4_define([rtsp_server_api_version],
          [rtsp_server_version_major.rtsp_server_version_minor])

AC_INIT(rtsp_server, rtsp_server_version)
AM_INIT_AUTOMAKE(rtsp_server, rtsp_server_version)
AC_CONFIG_HEADERS(config.h)

PKG_CHECK_MODULES([GSTREAMER], [gstreamer-0.10],
	   [have_gstreamer_0_10=yes])
PKG_CHECK_MODULES([GSTREAMERRTSP], [gstreamer-rtsp-0.10],
	   [have_gstreamer_rtsp_0_10=yes])

# Checks for programs.
AC_PROG_LIBTOOL
AM_PROG_CC_C_O
AC_PROG_INSTALL

AC_SUBST(rtsp_server_CFLAGS)
AC_SUBST(rtsp_server_LIBS)

AC_OUTPUT([
Makefile
src/Makefile
])

echo ""
echo "   rtsp_server $VERSION"
echo "   ====================="
echo ""
echo "   To build the project, run \"make\""
echo ""
