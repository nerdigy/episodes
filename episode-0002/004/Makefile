default: help

include build/*.mk

.PHONY: alpha # Target alpha
alpha:
	@echo "This is the first target"

.PHONY: bravo # Target bravo
bravo:
	@echo "This is the second target"

.PHONY: delta # Target delta
delta: alpha bravo
	@echo "This is the third target"
	@make four

help:
	@echo "Usage: make [target]"
	@echo ""
	@echo "Available targets:"
	@echo ""
	@cat $(MAKEFILE_LIST) | grep "^\.PHONY" | sed 's/\.PHONY: //' | sed 's/#/\t/g' | column -t -s $$'\t' | sort
	@echo ""
