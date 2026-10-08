
PROGRAMS = xv/xv xv/bggen xv/vdcomp xv/xcmap xv/xvpictoppm

CSOURCES1 = \
	xv/xv.c \
	xv/xvroot.c \
	xv/xvimage.c \
	xv/xvmisc.c \
	xv/xvbrowse.c \
	xv/xvinfo.c \
	xv/xvpopup.c \
	xv/xvbutt.c \
	xv/xvdial.c \
	xv/xvevent.c \
	xv/xvcut.c \
	xv/xvctrl.c \
	xv/xvscrl.c \
	xv/xvps.c \
	xv/xvdir.c \
	xv/xvpbm.c \
	xv/xvsunras.c \
	xv/xvgif.c \
	xv/xvxbm.c \
	xv/xvpm.c \
	xv/xvbmp.c \
	xv/xviris.c \
	xv/xvtarga.c \
	xv/xvxpm.c \
	xv/xvfits.c \
	xv/xvgam.c \
	xv/xvgraf.c \
	xv/xvgifwr.c \
	xv/xvcolor.c \
	xv/xvsmooth.c \
	xv/xv24to8.c \
	xv/xvtext.c \
	xv/xvalg.c \
	xv/xvdflt.c \
	xv/xvgrab.c \
	xv/xvrle.c \
	xv/xvpcx.c \
	xv/xviff.c \
	xv/xvxwd.c
COBJECTS1 = $(CSOURCES1:.c=.o)

CSOURCES2 = xv/bggen.c
COBJECTS2 = $(CSOURCES2:.c=.o)

CSOURCES3 = xv/vdcomp.c
COBJECTS3 = $(CSOURCES3:.c=.o)

CSOURCES4 = xv/xcmap.c
COBJECTS4 = $(CSOURCES4:.c=.o)

CSOURCES5 = xv/xvpictoppm.c
COBJECTS5 = $(CSOURCES5:.c=.o)

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

all: $(PROGRAMS)

xv/xv: $(COBJECTS1)
	$(LD) -o $@ $^ $(LDFLAGS)
xv/bggen: $(COBJECTS2)
	$(LD) -o $@ $^ $(LDFLAGS)
xv/vdcomp: $(COBJECTS3)
	$(LD) -o $@ $^
xv/xcmap: $(COBJECTS4)
	$(LD) -o $@ $^ $(LDFLAGS)
xv/xvpictoppm: $(COBJECTS5)
	$(LD) -o $@ $^

clean: objclean execlean
execlean:
	$(RM) $(PROGRAMS)
objclean:
	$(RM) $(COBJECTS1)
	$(RM) $(COBJECTS2)
	$(RM) $(COBJECTS3)
	$(RM) $(COBJECTS4)
	$(RM) $(COBJECTS5)

