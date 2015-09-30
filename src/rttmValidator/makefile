SHELL = /bin/sh
PREFIX=/Users/jfesslmeier/Downloads/sctk-2.4.0
bindir = $(PREFIX)/bin

all: rttmValidator.pl

rttmValidator.pl:
	chmod +x rttmValidator.pl

check: all
	(cd test_suite; $(SHELL) RunTest.sh ../rttmValidator.pl)

install: all
	cp rttmValidator.pl $(bindir)

clean:

distclean: clean
	rm -r *~ makefile
