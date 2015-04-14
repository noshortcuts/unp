include ../Make.defines

bin_PROGRAMS =	client clientrst \
		serv00 serv01 serv02 serv03 serv04 serv05 serv06 serv07 serv08 serv09 \
		serv02m serv02l serv03m


# The client to test the various servers.
client_SOURCES = 	client.c pr_cpu_time.c

# A special client that sends an RST occasionally.
# Used to test the XTI server (should receive disconnect).
clientrst_SOURCES = 	clientrst.c pr_cpu_time.c

# serv00_SOURCES =  traditional concurrent server_SOURCES =  use as base level
serv00_SOURCES = 	serv00.c web_child.c pr_cpu_time.c

# serv01_SOURCES =  one fork per client (traditional concurrent server).
serv01_SOURCES = 	serv01.c web_child.c sig_chld_waitpid.c pr_cpu_time.c

# serv02_SOURCES =  prefork, no locking; works on BSD-derived systems
#	but not on SVR4-derived systems.
serv02_SOURCES = 	serv02.c child02.c web_child.c pr_cpu_time.c

# serv02l_SOURCES =  prefork, no locking, block in select instead of accept to see
#	select collisions; works on BSD-derived systems but not on SVR4.
serv02l_SOURCES = serv02.c child02l.c web_child.c pr_cpu_time.c

# serv02m_SOURCES =  prefork, no locking; works on BSD-derived systems.
#	This version is "metered" to see #clients/child serviced.
serv02m_SOURCES = serv02m.c child02m.c web_child.c pr_cpu_time.c meter.c

# serv03_SOURCES =  prefork, file locking using fcntl().  Similar to Apache server.
serv03_SOURCES = 	serv03.c child03.c lock_fcntl.c web_child.c pr_cpu_time.c

# serv03m_SOURCES =  prefork, file locking using fcntl(), metered.
serv03m_SOURCES = 	serv03m.c child03m.c lock_fcntl.c web_child.c pr_cpu_time.c meter.c

# serv04_SOURCES =  prefork, file locking using pthread locking.
serv04_SOURCES = 	serv04.c child04.c lock_pthread.c web_child.c pr_cpu_time.c

# serv05_SOURCES =  prefork, descrptor passing to children.  Similar to NSCA server.
serv05_SOURCES = 	serv05.c child05.c lock_fcntl.c web_child.c pr_cpu_time.c

# Thread versions must call a reentrant version of readline().
# serv06_SOURCES =  one thread per client.
serv06_SOURCES = 	serv06.c web_child.c pr_cpu_time.c readline.c

# serv07_SOURCES =  prethread with mutex locking around accept().
serv07_SOURCES = 	serv07.c pthread07.c web_child.c pr_cpu_time.c readline.c

# serv08_SOURCES =  prethread with only main thread doing accept().
serv08_SOURCES = 	serv08.c pthread08.c web_child.c pr_cpu_time.c readline.c

# serv09_SOURCES =  prethread with no locking around accept().
serv09_SOURCES = 	serv09.c pthread09.c web_child.c pr_cpu_time.c readline.c

