
EXE = sphere_mac
OBJS = sphere.o makeSphere.o shader.o
FILES = sphere.c makeSphere.c shader.c
INCLUDES = /usr/X11R6/include -I /usr/include
LIB = /usr/X11R6/lib
LFLAGS = -lGL -lGLEW -lX11
CC = g++

.SUFFIXES: .c
prog: ${EXE}

#${EXE}: ${OBJS}
#	${CC} -L${LIB} -o $@ ${OBJS} ${LFLAGS}
#
#${OBJS}:${FILES}
#	 ${CC} -I${INCLUDES} -c ${FILES}
#another way to do it

.c.o:
	 ${CC} -I${INCLUDES} -c $<

${EXE}: ${OBJS}
	${CC} -L${LIB} -o $@ ${OBJS} ${LFLAGS}

clean:
	rm -f ${OBJS} ${EXE}
	make
