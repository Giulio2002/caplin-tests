# Caplin Tests files

This repository contains chain recordings in SSZ Snappy compressed format of historical data from ETH2.0 Mainnet. 
Those are meant to be used as regression/integration testing for the Caplin Consensus Layer.

## Regression tests format

tests for regression testing are under `regression`directory.

there are 2 types of files:

* Beacon States
* SignedBeaconBlock

Beacon state with id 0 is the starting state. each object has its raw hash bytes in `sidecar.bin` and the main 
payload in `data.bin`. Each block is to be executed sequentially and the process must be tested for 
performance/memory usage.
    
