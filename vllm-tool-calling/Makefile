NAMESPACE ?= vllm-tool-calling
MODEL ?= granite3.2-8b
PLATFORM ?= cpu

.PHONY: install uninstall

install:
	oc apply -k $(MODEL)/$(PLATFORM) -n $(NAMESPACE)

uninstall:
	oc delete -k $(MODEL)/$(PLATFORM) -n $(NAMESPACE) --ignore-not-found
