cc = g++
LFLAGS = -o
CFLAGS = -c -g -Wall -Werror
INC  = ./inc
IFLAG = -I$(Inc)
Bin = ./bin
OBJ = ./obj
SRC = ./src

all: employee

employee: $(OBJ)/employee.o
	$(CC) $(LFLAGS) $(BIN)/employee $(OBJ)/employee.o

$(OBJ)/employee.o: $(SRC)/employee.cpp
	$(CC) $(CFLAGS) $(IFLAG) $(SRC)/employee.cpp
	mv *.o $(OBJ)
clean:
	@echo "cleaning is in progress"
	rm -f a.out employee
	rm -f *.o
	rm -f $(OBJ)/*.o
	rm -f $(BIN)/employee
	@echo "done!
