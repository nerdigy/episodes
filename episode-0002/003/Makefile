default: help

include build/*.mk

.PHONY: alpha # Target alpha
alpha:
	@echo "This is the first target"

.PHONY: bravo # Target bravo
bravo:
	@echo "This is the second target"

.PHONY: charlie # Target charlie
charlie: alpha bravo
	@echo "This is the third target"
	@make four

.PHONY: help # Target help
help:
	@cat $(MAKEFILE_LIST) | grep "^\.PHONY"
