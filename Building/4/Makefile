SOURCES = main.cpp part1.cpp part2.cpp
OBJDIR = host
OBJECTS = ${addprefix ${OBJDIR}/,${SOURCES:.cpp=.o}}
EXECUTABLE = ${addprefix ${OBJDIR}/,parts}
CXX = g++

all: ${OBJECTS}
	${CXX} -o ${EXECUTABLE} ${OBJECTS}
	
${OBJDIR}/%.o: %.c
	${CXX} -c -o $@ $^
	
${OBJECTS}: | ${OBJDIR}
	
${OBJDIR}:
	@mkdir ${OBJDIR}
	
clean:
	@rm ${OBJECTS} ${EXECUTABLE}
	@rmdir ${OBJDIR}
	
help:
	@echo all clean help