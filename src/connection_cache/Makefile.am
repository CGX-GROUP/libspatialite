
SUBDIRS = generator

AM_CPPFLAGS = -I$(top_srcdir)/src/headers
AM_CPPFLAGS += @CFLAGS@ @CPPFLAGS@ @LIBXML2_CFLAGS@

noinst_HEADERS = cache_aux_1.h cache_aux_2.h cache_aux_3.h
noinst_LTLIBRARIES = libconnection_cache.la connection_cache.la

libconnection_cache_la_SOURCES = alloc_cache.c gg_sequence.c

connection_cache_la_SOURCES = alloc_cache.c gg_sequence.c 

connection_cache_la_CPPFLAGS = -I$(top_srcdir)/src/headers -I.
connection_cache_la_CPPFLAGS += @CFLAGS@ @CPPFLAGS@ @LIBXML2_CFLAGS@
connection_cache_la_CPPFLAGS += -DLOADABLE_EXTENSION
connection_cache_la_LDFLAGS = -module
connection_cache_la_LIBTOOLFLAGS = --tag=disable-static

MOSTLYCLEANFILES = *.gcna *.gcno *.gcda


