SOURCES = ../src/modbuslib.c ../src/common.c ../src/business.c ../src/main.c
HEADERS = ../src/data.h ../src/modbuslib.h ../src/common.h ../src/business.h ../src/thread.h
CC ?= gcc
LIBDIR ?= /usr/local/lib
INCDIR ?= /usr/local/include
DEBUGFLAG ?=
bdModbusGateway: $(SOURCES) $(HEADERS)
	$(CC) -o ../../$@ $(SOURCES) $(DEBUGFLAG) -I $(INCDIR) -L $(LIBDIR) -l:libcjson.a -lm -l:libmodbus.a -l:libssl.a -l:libcrypto.a -l:libpaho-mqtt3cs-static.a -lpthread -l:libssl.a -l:libcrypto.a -ldl

clean:
	rm ../../bdModbusGateway
