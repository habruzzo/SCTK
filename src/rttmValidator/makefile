SHELL = /bin/sh
PREFIX=/home/holden/proj-callr/athena/tools/SCTK
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
	$(RM) -r *~ makefile
