AC_INIT([libmongoose], [0.1], [luz@plan44.ch], [libmongoose], [http://www.plan44.ch/])
AC_PREREQ([2.59])

AC_CONFIG_AUX_DIR(configure_aux)
AC_CONFIG_MACRO_DIR([m4])

AM_INIT_AUTOMAKE([1.10 no-define foreign subdir-objects])
AC_CONFIG_HEADERS([config.h])

AC_PROG_CC
AC_PROG_CXX
AC_PROG_LIBTOOL

AC_CONFIG_FILES([Makefile])

AC_CHECK_LIB(dl, dlopen, [], [AC_MSG_ERROR([Could not find libdl])])

PKG_PROG_PKG_CONFIG

# Checks for header files.
AC_CHECK_HEADERS([arpa/inet.h assert.h ctype.h dirent.h dlfcn.h errno.h fcntl.h inttypes.h limits.h netdb.h netinet/in.h pwd.h signal.h stdarg.h stddef.h stdint.h stdio.h stdlib.h string.h sys/poll.h sys/socket.h sys/stat.h sys/time.h sys/types.h sys/wait.h time.h unistd.h], [], [AC_MSG_ERROR([required system header not found])])

CHECK_NETLINK

AX_PTHREAD([], [ AC_MSG_ERROR([required pthread library not found]) ])

AC_OUTPUT
