CC=gcc
CFLAGS=-g -Wall
CPPFLAGS=-I/usr/local/include
LDFLAGS=-L/usr/local/lib

OBJ=matrix.o bm-gen.o tournament.o ranking.o util.o unit_games.o partition.o blotto.o func.o
EXEC=bm-gen

%.o : %.c
	$(CC) -c $(CFLAGS) $(CPPFLAGS) $< -o $@

all: $(OBJ)
	$(CC) $(CFLAGS) $(OBJ) $(LDFLAGS) -o $(EXEC) -lgmp -lm

clean:
	rm $(OBJ) $(EXEC)
