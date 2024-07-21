default: help

include build/*.mk

one:
	@echo "This is the first target"

two:
	@echo "This is the second target"

three: one two
	@echo "This is the third target"
	@make four

help:
	@echo "This is the help target"
