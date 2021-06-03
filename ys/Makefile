out_dir := ../out
show_dir := show
stat_dir := stat

synth:
	$(shell if [ ! -e $(out_dir) ];then mkdir -p $(out_dir); fi)
	$(shell if [ ! -e $(show_dir) ];then mkdir -p $(show_dir); fi)
	$(shell if [ ! -e $(stat_dir) ];then mkdir -p $(stat_dir); fi)
	yosys -s synth.ys

clean:
	rm stat/*.txt
	rm show/*
	rm ../out/*.v
