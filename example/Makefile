#
# iniparser tests Makefile
#

CC      ?= gcc
CFLAGS  += -g -static -I../src
LFLAGS  += -L.. -liniparser
AR	    ?= ar
ARFLAGS += rcv
RM      ?= rm -f


default: all

all: iniexample parse

iniexample: iniexample.c
	$(CC) $(CFLAGS) -o iniexample iniexample.c ../src/iniparser.c

parse: parse.c
	$(CC) $(CFLAGS) -o parse parse.c ../src/iniparser.c

clean veryclean:
	$(RM) iniexample example.ini parse



