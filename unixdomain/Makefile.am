CFLAGS = -I ../include -Wall -g
LDADD = ../lib/libunp.a

bin_PROGRAMS =	daytimetcpcli daytimetcpsrv2 unixstrcli01 unixstrserv01 unixdgserv01 unixdgcli01 mycat \
	unixbind openfile
#	unixstrserv02 tfcred01

unixstrserv01_SOURCES = unixstrserv01.c sigchldwaitpid.c

#unixstrserv02_SOURCES = unixstrserv02.c strecho.c sigchldwaitpid.c readcred.c

mycat_SOURCES = mycat.c myopen.c
