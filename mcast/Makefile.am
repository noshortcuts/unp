include ../Make.defines

bin_PROGRAMS =	sendrecv udpcli01 udpcli05 udpcli06


sendrecv_SOURCES = 	main.c send.c recv.c

# Version in book.
udpcli01_SOURCES = 	udpcli01.c dgclibcast1.c

# Correct version using sigsetjmp()/siglongjmp().
udpcli05_SOURCES = 	udpcli05.c dgclimcast5.c

# Try to bind multicast address and send.
udpcli06_SOURCES = 	udpcli06.c dgclimcast6.c
