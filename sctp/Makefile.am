include ../Make.defines

bin_PROGRAMS =	sctpserv01 sctpclient01 sctpserv02 sctpserv03 sctpclient02 sctpserv04 \
sctpserv05 sctpclient03 sctpserv06 sctpserv07 sctpclient04 sctpserv_fork

#LIBS+= -L/usr/local/v6/lib -lm -lsctp

#.c.lc_SOURCES = 
#	../../troff/fixcode.sh $< > $@
#.h.lh_SOURCES = 
#	../../troff/fixcode.sh $< > $@

sctpclient01_SOURCES =    sctpclient01.c sctp_strcli.c sctp_strcliecho.c
sctpserv05_SOURCES = 	sctpserv05.c sctp_pdapircv.c 
sctpserv06_SOURCES = 	sctpserv06.c sctp_displayevents.c
sctpclient02_SOURCES = 	sctpclient02.c sctp_strcli.c sctp_strcliecho.c
sctpclient03_SOURCES =   sctpclient01.c sctp_strcli_un.c sctp_strcliecho.c
sctpserv07_SOURCES = 	sctpserv07.c sctp_displayevents.c sctp_bindargs.c 
sctpclient04_SOURCES = 	sctpclient04.c sctp_strcli1.c sctp_check_notify.c sctp_print_addrs.c sctp_modify_hb.c
sctpserv_fork_SOURCES =   sctpserv_fork.c sctp_addr_to_associd.c
