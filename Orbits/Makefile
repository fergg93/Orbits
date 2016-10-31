CXXFLAGS=-O3 -std=c++0x -Wall

SOURCES= $(wildcard *.cpp)

OBJECTS=$(patsubst %.cpp, %.o, $(SOURCES))

TARGET=$(lastword $(subst /, ,$(realpath .)))

LINKS= -lglut -lGL -lGLU

CXX=g++

all: $(TARGET)
	@echo Orbits built

$(TARGET): $(OBJECTS)
	@$(CXX) $(CXXFLAGS) -o Orbits $(OBJECTS) $(LINKS)

clean:
	rm -rf $(OBJECTS) $(TARGET)
