dactyls.far: dactyls.grm byte.far cmudict.far
	thraxcompiler --save_symbols --input_grammar=$< --output_far=$@

byte.far: byte.grm 
	thraxcompiler --save_symbols --input_grammar=$< --output_far=$@

cmudict.far: cmudict.grm cmudict.txt arpabet.sym cmudict.txt
	thraxcompiler --save_symbols --input_grammar=$< --output_far=$@

clean:
	rm -f byte.far cmudict.far
