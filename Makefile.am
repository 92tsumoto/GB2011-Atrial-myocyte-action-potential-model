#INCLUDES = syspara.h

bin_PROGRAMS = GB_atrial_2011
#GB_atrial_2011_CFLAGS = -O2 -Wall -axsse4.2 -mkl -parallel -par-report2 -Winline -inline-level=2 -ip -vec-report2 -opt-mem-layout-trans=3 -pg
GB_atrial_2011_CFLAGS = -O2 -Wall -axsse4.2 -mkl -parallel -par-report2 -vec-report2 -pg

GB_atrial_2011_INCLUDE = -I./include
GB_atrial_2011_LDADD = -L/opt/intel/mkl/lib/intel64 -liomp5 -lmkl_intel_lp64 -lmkl_intel_thread -lmkl_core ./lib/xhplot.o

GB_atrial_2011_SOURCES = ./src/GBd.c ./src/val_constants.c ./src/mem.c\
	./src/win_out.c ./src/eular.c ./src/runge.c ./src/input_para.c ./src/system.c ./src/currents.c\
	./src/eventloop.c ./src/exptable.c ./src/data_out.c ./src/syspara.h

