CC	= cc
CFLAGS	= -O
LDFLAGS	=

NAME	= philosopher
HDRS	= msecond.h random_int.h
OBJS	= $(NAME).o msecond.o random_int.o
LIBS	= -lpthread -lm
OUT	= $(NAME)

$(OUT):	$(OBJS)
	$(CC) $(LDFLAGS) -o $@ $(OBJS) $(LIBS)

$(NAME).o:	$(NAME).c $(HDRS)
msecond.o:	msecond.c msecond.h
random_int.o:	random_int.c random_int.h

clean:
	/bin/rm -f $(OBJS)

clobber:
	/bin/rm -f $(OBJS) $(OUT)
