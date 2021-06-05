MYPATH= $(shell find ../hs/dist-newstyle/ -type d -name potato |tail -n 1)

all: potatomain

potatomain: potatomain.cpp
	g++ -Wall -o $@ -I../hs/csrc $< -lpotato -L$(MYPATH)

run:
	LD_LIBRARY_PATH=$(MYPATH) ./potatomain

clean:
	rm -rf potatomain

.PHONY: clean all run

