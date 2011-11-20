fc = gfortran
source = cea2.f
cea2 : $(source)
	$(fc) -o cea2 -std=legacy $(source)
install:
	cp cea2 ../bin
clean : 
	rm -f cea2 