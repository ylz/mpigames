### Basic Makefile for MPI
CC			= /usr/bin/mpicc
CFLAGS 	= -g -O0
LD 			= /usr/bin/mpicc
LDFLAGS	= -g
PROGRAM	= hello-mpi
all:		${PROGRAM}
${PROGRAM}:		${PROGRAM}.o
							${LD} ${LDFLAGS} $< -o ${PROGRAM}
${PROGRAM}.o:	${PROGRAM}.c
							${CC} ${CFLAGS} -c $< -o ${PROGRAM}.o
clean:
							rm -f ${PROGRAM}.o ${PROGRAM}