output: dwmblocks.c blocks.h
	#cc `pkg-config --cflags x11` `pkg-config --libs x11` dwmblocks.c -o dwmblocks
	gcc -Wall -o dwmblocks dwmblocks.c -lX11
clean:
	rm -f *.o *.gch dwmblocks
install: output
	mkdir -p /usr/local/bin
	cp -f dwmblocks /usr/local/bin
