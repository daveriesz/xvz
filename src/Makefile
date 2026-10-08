
PROGRAM = xv/xv

CSOURCES = xv/xv.c xv/xvroot.c xv/xvimage.c xv/xvmisc.c xv/xvbrowse.c xv/xvinfo.c
COBJECTS = $(CSOURCES:.c=.o)

CC       = cc
CFLAGS   = $(COPT) $(CINC) $(CDEF)
COPT     = -g
CINC     = 
CDEF     = 

LD       = cc
LDFLAGS  = $(LDOPT) $(LDDIR) $(LDLIB)
LDOPT    = 
LDDIR    = 
LDLIB    = -lX11 -lm

all: $(PROGRAM)

$(PROGRAM): $(COBJECTS)
	$(LD) -o $@ $^ $(LDFLAGS)

