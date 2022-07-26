CC = g++
LFLAGS = -o
CFLAGS = -c -g -Wall -Werror
INC = ./inc
IFLAG = -I$(INC)
BIN = ./bin
OBJ = ./obj
SRC = ./src

all: multiassgnment

multiassgnment: $(OBJ)/multiassgnment.o
	$(CC) $(LFLAGS) $(BIN)/multiassgnment $(OBJ)/multiassgnment.o

$(OBJ)/multiassgnment.o: $(SRC)/multiassgnment.cpp
	$(CC) $(CFLAGS) $(IFLAG) $(SRC)/multiassgnment.cpp 
	mv *.o $(OBJ)


clean:
	@echo "Cleaning is in Progress"
	rm -f a.out multiassgnment
	rm -f *.o
	rm -f $(OBJ)/*.o
	rm -f $(BIN)/multiassgnment
	@echo "Done!"
													

