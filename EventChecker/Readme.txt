how to compile:

gcc -O3 -Wall -c -fmessage-length=0 -o DateValidation.o DateValidation.c
gcc -shared -o timedll.dll DateValidation.o
gcc -o test_eventchecker DllTest.c -L./ -ltimedll

put time.txt in the same folder as the dll.
time in GMT/UTC
format:  yyyy-mm-dd hh:MM:ss
