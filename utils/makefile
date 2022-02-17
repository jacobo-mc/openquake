
# Define all the project (directories) to build
PROJECTS += mdl2map
PROJECTS += mesh2map 
PROJECTS += mkwad
PROJECTS += par
PROJECTS += pcx2lmp
PROJECTS += qutils 
PROJECTS += toon
PROJECTS += tri2map

.PHONY : $(PROJECTS)

all : $(PROJECTS)

#
# for each project, run "make" in the directory by that name
#
$(PROJECTS) :
	$(MAKE) -C $@


#
# For each project, define a "project.clean" target the cleans
# that directory.
#
CLEANTARGETS = $(addsuffix .clean, $(PROJECTS))

clean : $(CLEANTARGETS) ;

%.clean :
	$(MAKE) -C $* clean

