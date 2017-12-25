gcc -O3 -Wall -c -fmessage-length=0 -o DateValidation.o DateValidation.c

gcc -shared -o timedll.dll DateValidation.o


gcc -o test DllTest.c -L./ -ltimedll
