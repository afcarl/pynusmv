## Makefile.am generated by the makefiler script
##
# FileName	[ Makefile ]
#
# PackageName	[ NuSMV ]
#
# Synopsis	[ Package-wide Makefile ]
#
# Description	[ Makefile template for the NuSMV executable ]
#
# Author	[ Alessandro Mariotti ]
#
# Copyright	[This file is part of the ``wff'' package of NuSMV 
#  version 2. Copyright (C) 2011 by FBK-irst. 
#
#  NuSMV version 2 is free software; you can redistribute it and/or 
#  modify it under the terms of the GNU Lesser General Public 
#  License as published by the Free Software Foundation; either 
#  version 2 of the License, or (at your option) any later version.
#
#  NuSMV version 2 is distributed in the hope that it will be useful, 
#  but WITHOUT ANY WARRANTY; without even the implied warranty of 
#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU 
#  Lesser General Public License for more details.
#
#  You should have received a copy of the GNU Lesser General Public 
#  License along with this library; if not, write to the Free Software 
#  Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA.
#
#  For more information on NuSMV see <http://nusmv.fbk.eu>
#  or email to <nusmv-users@fbk.eu>.
#  Please report bugs to <nusmv-users@fbk.eu>.
#
#  To contact the NuSMV development board, email to <nusmv@fbk.eu>. ]
#

AUTOMAKE_OPTIONS = subdir-objects

SUBDIRS = w2w

CUDD_NAME = $(cuddname)
CUDD_DIR = ../$(CUDD_NAME)

INCLUDES = -I. -I.. -I$(top_srcdir)/src -I$(top_srcdir)/$(CUDD_DIR)/include

wff_HEADERS = wff.h
PKG_SOURCES = wffPkg.c exprWff.c $(wff_HEADERS)

wffdir = $(includedir)/nusmv/wff

# -------------------------------------------------------

noinst_LTLIBRARIES = libwff.la
libwff_la_SOURCES = $(PKG_SOURCES)

libwff_la_LIBADD = w2w/libw2w.la
