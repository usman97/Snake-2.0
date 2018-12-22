PY = python3
DOXY = doxygen
DOXYCFG = doxConfig

RMDIR = rm -rf

.PHONY: test doc clean

test:
	$(PY) ../../../src/*

doc:
	$(DOXY) $(DOXYCFG)
	cd latex && $(MAKE)
  
clean:
	@- $(RMDIR) html
	@- $(RMDIR) latex
