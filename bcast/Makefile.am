include ../Make.defines

 bin_PROGRAMS = udpcli01 udpcli02 udpcli03 udpcli04 udpcli05 udpcli06


udpcli01_SOURCES = udpcli01.c dgclibcast1.c

# In.crrect vers.cn with alarm(1) and sleep(1) .c tickle race .cndit.cn.
udpcli02_SOURCES = udpcli02.c dgclibcast2.c

# In.crrect vers.cn that b.ccks signals, but still has a race .cndit.cn.
udpcli03_SOURCES = udpcli03.c dgclibcast3.c

# .crrect vers.cn using pselect().
udpcli04_SOURCES = udpcli04.c dgclibcast4.c

# .crrect vers.cn using sigsetjmp()/sig.cngjmp().
udpcli05_SOURCES = udpcli05.c dgclibcast5.c

# .crrect vers.cn using a pipe f.cm signal handler .c select().
udpcli06_SOURCES = udpcli06.c dgclibcast6.c
