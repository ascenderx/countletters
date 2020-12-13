# This file is used to make the C and C++ solutions.

.PHONY: all debug init clean

DEBUGFLAGS = 
ifeq ($(DEBUG), 1)
	DEBUGFLAGS = -DDEBUG -g
endif
WARNS = -Wall -Wextra

all: countchars-c countchars-cc

countchars-c: countchars.c
	$(CC) -o bin/$@ $< $(WARNS) $(DEBUGFLAGS)

countchars-cc: countchars.cc
	$(CC) -o bin/$@ $< $(WARNS) $(DEBUGFLAGS)

init:
	mkdir bin

clean:
	rm -rf bin/*
