# CIS Benchmark Evaluation

This repository is part of the paper *Automated Implementation of Windows-related Security-Configuration Guides* presented at the 35th IEEE/ACM International Conference on Automated Software Engineering.
In this repository, we have collected our evaluation data using 12 benchmarks of the [Center for Internet Security (CIS)](https://www.cisecurity.org/).
For each benchmark:

1. We have set up a clean VM with the tested OS.
If the tested software was not an OS, we installed the software on a Windows 10 instance.
2. We installed the [CIS-CAT tool](https://www.cisecurity.org/cybersecurity-tools/cis-cat-pro/) on the VM.
3. We executed the OVAL checks of the tested CIS benchmark with the CIS-CAT tool on the VM.
The results are stored as `before.html`, e.g., [for Windows 10](https://github.com/tum-i22/CIS-Benchmark-Evaluation/blob/master/cis_win_10_1806/before.html).
4. Next, we executed the automatic remediation of the benchmark using our generated scripts.
5. Finally, we reran the OVAL checks.
This time, the results are stored as `after.html`, e.g., [for Windows 10](https://github.com/tum-i22/CIS-Benchmark-Evaluation/blob/master/cis_win_10_1806/after.html).

You can download the benchmarks in their PDF from the [CIS website](https://www.cisecurity.org/cis-benchmarks/).

If you have any questions, please create an issue or contact [Patrick Stöckle](mailto:patrick.stoeckle@tum.de).

Please also have a look at

* [DISA Windows Server 2016 STIG Evaluation](https://github.com/tum-i22/disa-windows-server-2016)
* [DISA Windows Server 2019 STIG Evaluation](https://github.com/tum-i22/disa-windows-server-2019)
