#
# Makefile ESQUELETO
#
# DEVE ter uma regra "all" para geração da biblioteca
# regra "clean" para remover todos os objetos gerados.
#
# NECESSARIO adaptar este esqueleto de makefile para suas necessidades.
#
#

CC=gcc
LIB=-lt2fs
LIB_DIR=../lib/
INC_DIR=../include/
BIN_DIR=../bin/
SRC_DIR=../src/
CFLAGSObj=-m32 -c
CFLAGSExe=-m32 -o

all: create init identify diskDissection

create:
	$(CC) $(CFLAGSExe) $(BIN_DIR)create create.c -L$(LIB_DIR) $(LIB)

init:
	$(CC) $(CFLAGSExe) $(BIN_DIR)init init.c -L$(LIB_DIR) $(LIB)

identify:
	$(CC) $(CFLAGSExe) $(BIN_DIR)identify identify.c -L$(LIB_DIR) $(LIB) 

diskDissection:
	$(CC) $(CFLAGSExe) $(BIN_DIR)diskDissection diskDissection.c -L$(LIB_DIR) $(LIB)

clean:
	find $(BIN_DIR) -type f ! -name 't2fs_disk.dat' ! -name 't2fs.o' -delete
