SOURCES = main.cpp part1.cpp part2.cpp
DIR = host/
OBJECTS = ${SOURCES:%.cpp=${DIR}%.o}
EXECUTABLE = ${DIR}parts
CXX = g++

all: makedir ${OBJECTS}
	${CXX} -o ${EXECUTABLE} ${OBJECTS}
	
makedir: 
	@mkdir ${DIR}
	
${DIR}%.o: %.cpp
	${CXX} -c -o $@ $^

clean:
	@rm ${OBJECTS} ${EXECUTABLE}
	@rmdir ${DIR}

help:
	@echo all clean help