CC=gcc


CFLAGS= -O2 -g -Wall -I../../../include -I../UctDspLib -I../../ParseParams
LDFLAGS= -lpowerdaq32

TARGET=DspMeasPeriod
OBJECTS=../UctDspLib/powerdaq_Uct.o DspMeasPeriod.o ../../ParseParams/ParseParams.o

all:  $(TARGET)

$(TARGET): $(OBJECTS)
	$(CC) $(OBJECTS) $(LDFLAGS) -o $@ 
	
.c.o:
	$(CC) -c $(CFLAGS) -c $< -o $@
	
clean:
	rm -f $(OBJECTS)
	rm -f $(TARGET)
