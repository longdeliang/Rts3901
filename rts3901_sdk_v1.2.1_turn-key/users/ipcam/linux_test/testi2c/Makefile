#
# Realtek Semiconductor Corp.
#
# peter_sun (peter_sun@realsil.com.cn)
# Oct. 31, 2014
#

SRCS=testi2c.c
OUTPUT=testi2c

all: $(OUTPUT)

$(OUTPUT):$(SRCS:.c=.o)
	$(CC) $(LDFLAGS) $(LIBS) $^ -o $@
	$(STRIP) $@

romfs:
	$(ROMFSINST) $(OUTPUT) /bin/$(OUTPUT)

clean:
	rm -f $(OUTPUT)
