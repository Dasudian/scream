LIBSRC=VideoEnc.cpp RtpQueue.cpp NetQueue.cpp ScreamTx.cpp ScreamRx.cpp
LIB=libscream.a
CC=g++
CFLAGS := `pkg-config glib-2.0 --cflags --libs`
CFLAGS += -std=c++11
TARGET=scream_01 scream_02 scream_03

all:rm $(TARGET)

rm:
	$(RM) $(TARGET)
	
scream_01:scream_01.cpp $(LIBSRC)
	$(CC) -o $@ $^ $(CFLAGS)

scream_02:scream_02.cpp $(LIBSRC)
	$(CC) -o $@ $^ $(CFLAGS)

scream_03:scream_03.cpp $(LIBSRC)
	$(CC) -o $@ $^ $(CFLAGS)

.PHONY : clean
clean:
	$(RM) $(TARGET)