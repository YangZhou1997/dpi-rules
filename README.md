# dpi-rules

* `rawrules/`: contains raw snort rules from https://www.snort.org/downloads and  https://rules.emergingthreats.net/fwrules/.
* `rules/words.rules`: split() the sentense rules
* `rules/regex.rules`: extracted from the pcre field of raw rules, dedup.

* `rules/sentense.rules`: extracted from the contents field of raw rules, dedup; used by netbricks/dpi. 
* `rules/hs.rules`: generated from sentense rules, used by netbricks/hyperscan
* `rules/dpirules.rs`: generated from sentense rules, used by safebricks/dpi and netbricks-gem5/dpi
* `rules/dpihsrules.rs`: generated from sentense rules, used by safebricks/hyperscan and netbricks-gem5/hyperscan
