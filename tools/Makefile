CFLAGS=-g
LIBS=-lwsock32
CC=gcc

BINS= \
	dump_lv2_pcap_to_bin.exe \
	dump_elfs_pcap_to_dir.exe \
	bin2header.exe
SRCS= \
	dump_lv2_pcap_to_bin.c \
	dump_elfs_pcap_to_dir.c \
	bin2header.c

%.exe: %.c
	$(CC) $(CFLAGS) -o $@ $< $(LIBS)

all: $(BINS)

clean:
	rm -f $(BINS) *~
