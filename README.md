# This is my README

Two scritps are used to generate the reports

1. src/run
2. src/backtrace

`src/run` is a wrapper, it is responsible for connecting to a set of remote hosts, executing `src/backtrace` and emailing a crash report.

`src/backtrace` checks for new core files since it last ran, it uses _gdb_ to collect a backtrace, and then marks the corefile to exclude it from a subsequent request from the runner.


