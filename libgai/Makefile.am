include ../Make.defines

# Note: In the source code in this directory I #ifdef the constants
# IPv4, IPv6 (both lowercase "v"), and UNIXdomain.  This is instead of
# the all-uppercase constants so that these #ifdef/#endif lines do not
# appear in the book (too much clutter, given the amount of conditional
# testing for all the code in this directory).

noinst_LIBRARIES = libgai.a
libgai_a_SOURCES =  ga_aistruct.c ga_clone.c ga_echeck.c ga_nsearch.c ga_port.c ga_serv.c gn_ipv46.c \
					freeaddrinfo.c gai_strerror.c
#					getnameinfo.c ga_unix.c getaddrinfo.c
bin_PROGRAMS = testga test1
