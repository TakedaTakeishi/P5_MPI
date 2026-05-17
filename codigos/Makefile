CC = mpicc
CFLAGS = -Wall -Wextra -O3
LDFLAGS = 

TARGET = main
SRC = main.c

all: $(TARGET)

$(TARGET): $(SRC)
	$(CC) $(CFLAGS) -o $(TARGET) $(SRC) $(LDFLAGS)

run: $(TARGET)
	mpirun --mca btl ^tcp -np 8 ./$(TARGET)

clean:
	rm -f $(TARGET)

.PHONY: all run clean
