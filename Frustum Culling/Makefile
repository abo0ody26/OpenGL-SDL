CC			= g++

TARGET		= FrustumCulling

$(TARGET):	Main.o Init.o Frustum.o Camera.o
	$(CC) -o $(TARGET) Main.o Init.o Frustum.o Camera.o `sdl-config --libs` -lGL -lGLU -lm

Main.o:		Main.cpp main.h
	$(CC) -c Main.cpp `sdl-co ig --cflags`

Frustum.o:  Frustum.cpp main.h
	$(CC) -c Frustum.cpp `sdl-config --cflags`

Camera.o:   Camera.cpp Camera.h
	$(CC) -c Camera.cpp `sdl-config --cflags`

Init.o:		Init.cpp main.h
	$(CC) -c Init.cpp `sdl-config --cflags`

clean:
	rm -f $(TARGET) Main.o Init.o Frustum.o Camera.o core
