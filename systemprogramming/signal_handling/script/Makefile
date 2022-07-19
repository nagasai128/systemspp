CC = g++
LFLAGS = -o
CFLAGS = -c -g -Wall -Werror
INC = ./inc
IFLAG = -I$(INC)
BIN = ./bin
OBJ = ./obj
SRC = ./src

all: signal

signal: $(OBJ)/signal.o
		$(CC) $(LFLAGS) $(BIN)/signal $(OBJ)/signal.o

$(OBJ)/signal.o: $(SRC)/signal.cpp
		$(CC) $(CFLAGS) $(IFLAG) $(SRC)/signal.cpp 
			mv *.o $(OBJ)


clean:
	@echo "Cleaning is in Progress"
	rm -f a.out signal
	rm -f *.o
	rm -f $(OBJ)/*.o
	rm -f $(BIN)/signal
	@echo "Done!"
