
.PHONY: all clean run install uninstall doc tar cleanall help start
DIR=/home/01/esavinov/Dimon/0/1
	
all: hello
	
clean:
			rm -rf *.o
cleanall:	
			rm -rf *.o manual.txt hello 1 *gz
main.o: main.c
			gcc -c -o main.o main.c
hello.o: hello.c
			gcc -c -o hello.o hello.c
hello: main.o hello.o
			gcc -o hello main.o hello.o
run: 
			@./1
install:
			install ./hello $(DIR)
uninstall:
			rm -rf $(DIR)
doc : 			
			cat readme.txt control.txt > manual.txt
tar: 			
			tar -cf hello.tar.gz main.c hello.c readme.txt control.txt makefile; 
help:
			@echo 'clean - Очистить лишнее; help - помощь; doc - документация; install - Установка;'
start:			
			@./hello
%::
			@echo 'clean - Очистить лишнее; help - помощь; doc - документация; install - Установка;'
