fc = gfortran
source = cea2.f
program = cea2
cea2 : $(source)
	$(fc) -o $(program) -std=legacy $(source)
libs : cea2
	./$(program) < thermo.inp > /dev/null
	./$(program) < trans.inp > /dev/null
install: cea2 libs
	cp $(program) ../bin
	cp thermo.lib ../bin
	cp trans.lib ../bin
clean : 
	rm -f $(program)
cleanall:
	rm -f $(program) thermo.lib trans.lib