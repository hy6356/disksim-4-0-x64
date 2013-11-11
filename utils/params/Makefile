
# DiskSim Storage Subsystem Simulation Environment (Version 4.0)
# Revision Authors: John Bucy, Greg Ganger
# Contributors: John Griffin, Jiri Schindler, Steve Schlosser
#
# Copyright (c) of Carnegie Mellon University, 2001-2008.
#
# This software is being provided by the copyright holders under the
# following license. By obtaining, using and/or copying this software,
# you agree that you have read, understood, and will comply with the
# following terms and conditions:
#
# Permission to reproduce, use, and prepare derivative works of this
# software is granted provided the copyright and "No Warranty" statements
# are included with all reproductions and derivative works and associated
# documentation. This software may also be redistributed without charge
# provided that the copyright and "No Warranty" statements are included
# in all redistributions.
#
# NO WARRANTY. THIS SOFTWARE IS FURNISHED ON AN "AS IS" BASIS.
# CARNEGIE MELLON UNIVERSITY MAKES NO WARRANTIES OF ANY KIND, EITHER
# EXPRESSED OR IMPLIED AS TO THE MATTER INCLUDING, BUT NOT LIMITED
# TO: WARRANTY OF FITNESS FOR PURPOSE OR MERCHANTABILITY, EXCLUSIVITY
# OF RESULTS OR RESULTS OBTAINED FROM USE OF THIS SOFTWARE. CARNEGIE
# MELLON UNIVERSITY DOES NOT MAKE ANY WARRANTY OF ANY KIND WITH RESPECT
# TO FREEDOM FROM PATENT, TRADEMARK, OR COPYRIGHT INFRINGEMENT.
# COPYRIGHT HOLDERS WILL BEAR NO LIABILITY FOR ANY USE OF THIS SOFTWARE
# OR DOCUMENTATION.

all: $(TARGETS)

include .paths

<<<<<<< HEAD
DISKSIM_CFLAGS=-m32 -I../../src
DISKSIM_LDFLAGS=-m32 -L../../src -ldisksim

CFLAGS = -g -fPIC -m32\
=======
DISKSIM_CFLAGS=-I../../src
DISKSIM_LDFLAGS=-L../../src -ldisksim

CFLAGS = -g \
>>>>>>> b2a7ef9da759b6df9438c96bab636aa1cfb36ecc
        $(DISKSIM_CFLAGS) \
        $(DISKMODEL_CFLAGS) \
        $(LIBPARAM_CFLAGS) \
        $(LIBDDBG_CFLAGS) 

<<<<<<< HEAD
LDFLAGS = -m32 $(DISKSIM_LDFLAGS) \
=======
LDFLAGS = $(DISKSIM_LDFLAGS) \
>>>>>>> b2a7ef9da759b6df9438c96bab636aa1cfb36ecc
	  $(DISKMODEL_LDFLAGS) \
          $(LIBPARAM_LDFLAGS) \
          $(LIBDDBG_LDFLAGS) -lm

TARGETS = merge_blocks libparam_to_v3
all: $(TARGETS)

merge_blocks: merge_blocks.o
	$(CC) $(CFLAGS) $^ -o $@ $(LDFLAGS)

libparam_to_v3: libparam_to_v3.o
	$(CC) $(CFLAGS) $^ -o $@ $(LDFLAGS)


clean:
	rm -f *.o $(TARGETS)
distclean: clean
