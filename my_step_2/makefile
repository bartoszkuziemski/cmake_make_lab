# Makefile for Writing Make Files Example
 
# *****************************************************
# Variables to control Makefile operation
 
CC = g++
CFLAGS = -Wall -g
 
# ****************************************************
# Targets needed to bring the executable up to date
 
main: main.o Polygon.o Rectangle.o Triangle.o
    $(CC) $(CFLAGS) -o main main.o Polygon.o Rectangle.o Triangle.o
 
# The main.o target can be written more simply
 
main.o: main.cpp Polygon.h Rectangle.h Triangle.h
    $(CC) $(CFLAGS) -c main.cpp
 
Polygon.o: Polygon.h
 
Rectangle.o: Rectangle.h Polygon.h

Triangle.o: Triangle.h Polygon.h
