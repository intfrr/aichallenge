#Archive the starter packs

STARTER_BOTS = $(wildcard starter_bots/*/)
STARTER_PACKAGES = $(STARTER_BOTS:starter_bots/%/=%.zip)

all: archives

archives: $(STARTER_PACKAGES)

%.zip: starter_bots/%/
	zip -r $@ $<

clean:
	-rm -Rf $(STARTER_PACKAGES)

.PHONY: archives all clean