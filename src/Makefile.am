AM_CFLAGS         = -Wall -Wcast-align 

bin_PROGRAMS      = pbmtodp
pbmtodp_SOURCES   = pbmtodp.c
pbmtodp_LDFLAGS   = 

bin_SCRIPTS       = intermec-dp-drv

intermecppddir    = ${prefix}/share/cups/model/intermec
intermecppd_DATA  = ppd/*.ppd

ppd/*.ppd:
	ppdc -d ppd generic-dp.drv

clean-local:
	rm ppd/*
