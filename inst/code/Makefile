# The C compiler to use.
CC=gcc

# The location of the libgit2 include files.
LIBGIT2_INCLUDE=/usr/local/Cellar/libgit2/0.27.7/include

# RULES
# -----
all: git_log

common.o: common.c
	$(CC) -c $^ -I$(LIBGIT2_INCLUDE)

log.o: log.c
	$(CC) -c $^ -I$(LIBGIT2_INCLUDE)

#/ gcc -c log.c -I/usr/local/Cellar/libgit2/0.27.7/include
# gcc -o gitlog common.o log.o -L/usr/local/Cellar/libgit2/0.27.7/lib -lgit2

clean:
	rm -f git_log common.o log.o


