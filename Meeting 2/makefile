# Variables
CXX = g++
CXXFLAGS = -Wall
TARGET = Meeting2
TARGETTEST = Meeting2
SRC = Meeting2.cpp
SRCTEST = Meeting2.cpp

# Default target: compile the program
all: $(TARGET)

# Compile the sum.cpp 	
$(TARGET): $(SRC)
	$(CXX) $(CXXFLAGS) -o $(TARGET) $(SRC)

# Run the program
run: $(TARGET)
	./$(TARGET)

# Clean up the compiled files
clean:
	rm -f $(TARGET)
	rm -f $(TARGETTEST)

test: ${TARGETTEST}

$(TARGETTEST): $(SRCTEST)
	$(CXX) $(CXXFLAGS) -o $(TARGETTEST) $(SRCTEST)
	./$(TARGETTEST)

# Phony targets to avoid conflicts
.PHONY: all clean test