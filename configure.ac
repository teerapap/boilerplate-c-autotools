dnl Process this file with autoconf to produce a configure script.

AC_PREREQ(2.59)
AC_INIT([woof], [0.1.0-pre-alpha-0], [teerapap.c@gmail.com])

AC_CONFIG_AUX_DIR([build-aux])
AC_CONFIG_MACRO_DIR([m4])

AC_CANONICAL_SYSTEM
AM_INIT_AUTOMAKE([foreign -Wall -Werror])

AC_PROG_CC

dnl this allows us specify individual liking flags for each target
AM_PROG_CC_C_O 

dnl Initialize Libtool
LT_INIT

dnl Check if Libtool is present
dnl Libtool is used for building share libraries 
AC_PROG_LIBTOOL

AC_CONFIG_FILES(Makefile 
                src/Makefile
                deps/Makefile
                doc/Makefile
                test/Makefile
                )

dnl Dependencies build
dnl AC_CONFIG_SUBDIRS([deps/dep1])

AC_OUTPUT

