[![](https://img.shields.io/badge/AIGer-v1.9.4-1E90FF.svg)](https://fmv.jku.at/aiger/)
[![](https://img.shields.io/badge/berkeley_abc-ff6156.svg)](https://github.com/berkeley-abc/abc)
[![](https://img.shields.io/badge/aiger_format-6611f8.svg)](https://fmv.jku.at/aiger/FORMAT)
# Blif-to-AIGer
## Introduction
This is a low level synthesis tool. It implements the "structural hashing" (strashing) algorithm for constructing And-Inverter-Graphs (AIGs).

This tool can read Boolean functions from BLIF files. The constructed AIGs is written out in the
ASCII AIGER format (.aag). Java is the main language. To transfer it to the binary AIGer 
format (.aig file), which can be read directly by tool **ABC**, AIGer tool **aigtoaig** can be used.

## Test
To evaluate the implementation, an equivalence check of the input BLIF files and the resulting AIGs shall be performed with ABC.
Furthermore, the number of nodes in the AIGs shall be evaluated.