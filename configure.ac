AC_INIT([opvp_null], [0.0.1])
AC_CONFIG_SRCDIR([opvp_null.c])
AM_INIT_AUTOMAKE
AM_CONFIG_HEADER([config.h])

AC_CONFIG_MACRO_DIR([m4])

AC_ARG_ENABLE(debug)
if test x"${enable_debug}" = xyes; then
  CFLAGS="${CFLAGS} -DDEBUG_PRINT"
fi

AC_ARG_ENABLE(progpath)
AC_DEFINE([PROG_PATH], [$enable_progpath], [Define if needed])
AC_SUBST(PROG_PATH)

# Checks for programs.
AC_PROG_CXX
AC_PROG_CC
AC_PROG_LN_S
AC_PROG_MAKE_SET
AM_PROG_LIBTOOL

# Checks for libraries.

# Checks for header files.
AC_HEADER_STDC
AC_CHECK_HEADERS([stdlib.h string.h unistd.h stdarg.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_HEADER_STDBOOL
AC_C_CONST

# Checks for library functions.
AC_FUNC_MALLOC
AC_FUNC_MEMCMP
AC_FUNC_VPRINTF
AC_CHECK_FUNCS([memset])

# AC_CONFIG_FILES([Makefile])
AC_OUTPUT([Makefile])
