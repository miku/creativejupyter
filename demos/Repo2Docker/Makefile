Dockerfile:
	jupyter-repo2docker --no-build --debug /home/tir/code/norvig/pytudes 2>&1 | tail -n +5 > $@

.PHONY: run
run:
	jupyter-repo2docker /home/tir/code/norvig/pytudes 2>&1

.PHONY: clean
clean:
	rm -f Dockerfile

