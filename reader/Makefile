EXEC = com_reader
OBJS = com_reader.o uart_api.o
HEADERS = uart_api.h

HOST_CC = gcc
TARGET_CC = arm-linux-gcc
CC = ${TARGET_CC}

INC = -I.
CFLAGS = ${INC} -g 

all:${EXEC}
${EXEC} : ${OBJS}
	${CC} ${CFLAGS} ${LDFLAGS} -o $@ ${OBJS} 
${OBJS2} : ${HEADERS}

.PHONY : clean
clean :
	-rm -f ${OBJS} ${EXEC}
