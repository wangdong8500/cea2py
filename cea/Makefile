fc = gfortran
source = cea2.f
program = cea2
cea2 : $(source)
	$(fc) -o $(program) -std=legacy $(source)
install:
	cp   $(program) ../bin
libs :
	./$(program) thermo
	./$(program) trans
clean : 
	rm -f $(program)
cleanall:
	rm -f $(program) thermo.lib trans.lib