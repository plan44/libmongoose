AUTOMAKE_OPTIONS = subdir-objects
ACLOCAL_AMFLAGS = ${ACLOCAL_FLAGS} -I m4

lib_LTLIBRARIES = libmongoose.la

# libmongoose

libmongoose_la_CFLAGS =

libmongoose_la_CPPFLAGS = \
  -D RASPBERRY_PI=1 \
  -D_GNU_SOURCE=1

libmongoose_la_SOURCES = \
  mongoose.c \
  mongoose.h
