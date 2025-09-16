# Compiler and flags
CC = gcc
CFLAGS = -Wall -Werror -I./src

# Files
SRC = src/main.c src/add.c
OBJ = $(SRC:.c=.o)
TARGET = my_program

# Default target
all: $(TARGET)

# Link object files into executable
$(TARGET): $(OBJ)
	$(CC) $(OBJ) -o $(TARGET)

# Compile each .c to .o
%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

# Clean build files
clean:
	rm -f $(OBJ) $(TARGET)
