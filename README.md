# container

this 'container' project is an example of submodules usage with sample repos.

each submodule is a subdirectory with git repository that points to a single (headless) commit,
that way it's easy to track changes.

each repo should have a 'release' branch, so we can pull everything with:
	
	git submodule foreach 'git checkout -b release'
	git submodule foreach 'make'

the container should be empty, apart from common files as .idl files

# future ideas

* use automation testing server like Travis/Jenkins etc.
* use drivepx as a remote, push for testing