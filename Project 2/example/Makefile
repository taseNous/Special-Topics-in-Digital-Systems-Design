.DEFAULT_GOAL:=help
######################################################
synthesis:
	dc_shell -f run.tcl | tee syn.log
######################################################
.PHONY: synthesis
######################################################
atpg:
	tmax -shell -notcl tmax.script | tee tmax.log
######################################################
.PHONY: atpg
######################################################
help:
	cat README
######################################################
.PHONY:help
######################################################
clean:
	$(RM) -r WORK *.log *.svf *.sdf \
	*_netlist.* *.sdc *.spf *_synth.v \
	*_myvectors.v *.dat
######################################################
.PHONY:help
######################################################
