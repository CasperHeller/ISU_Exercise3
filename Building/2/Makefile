SOURCES = hello.cpp
OBJECTS= ${SOURCES:.cpp=.o}
EXECUTABLE = hello
CXX = g++

all: ${OBJECTS}
	${CXX} -o ${EXECUTABLE} ${OBJECTS}
	
%.o: %.cpp
	${CXX} -c -o $@ $^

clean:
	@rm ${OBJECTS} ${EXECUTABLE}
	
help:
	@echo all clean help