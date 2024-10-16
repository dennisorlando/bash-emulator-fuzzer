# bash-emulator-fuzzer
The purpose of this repository is to run most of the Bash' unit tests against a might-be Bash emulator, in order to find bugs or anomalous behaviours.
The main intent behind this repo is to nuke-fingerprint non-pure SSH honeypots in order to show that they are completely useless against fingerprinting attacks.

### Usage
This repository contains a pre-generated `tests.tar` file generated from `tar cf tests.tar tests/`.
To run the tests, login into your shell / emulator, extract the tests and run `run-all`.
You will be greeted with a ton of unintuinive logs which the official bash repository didn't mention to explain.
A fully functional bash shell should spit out only the names of the scripts being run, while any other output can be regardere as a failure.
Here is an example of running the tests on my laptop, i.e. with a working shell:
