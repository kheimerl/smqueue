#
# Copyright 2008 Free Software Foundation, Inc.
#
# This software is distributed under the terms of the GNU Public License.
# See the COPYING file in the main directory for details.
#
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <http://www.gnu.org/licenses/>.
#

include $(top_srcdir)/Makefile.common

AM_CPPFLAGS = $(STD_DEFINES_AND_INCLUDES)
AM_CXXFLAGS = -Wall -g -losipparser2 -losip2 -lc -lpthread

noinst_PROGRAMS = \
	smtest \
	smrelaytest \
	sminterface

smtest_SOURCES = \
	smtest.cpp 
smtest_LDADD = \
	$(COMMON_LA) \
	$(SQLITE_LA)

smrelaytest_SOURCES = \
	smrelaytest.cpp
smrelaytest_LDADD = \
	$(COMMON_LA) \
	$(SQLITE_LA)

sminterface_SOURCES = \
	sminterface.cpp
sminterface_LDADD = \
	$(COMMON_LA) \
	$(SQLITE_LA)

EXTRA_DIST = \
	smtest.h \
	smrelaytest.h

