# submodule-contract-artifacts
This repository keeps hardhat artifacts of deployed contacts on different chains. Artifacts have addresses, code, contructor arguments, chainid of deployed contracts.

We use separate repository to have ability to use it in multiple projects simultaneously as [git-submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules), such as contract and UI repositories.

The workflow: in contract's repo - contracts get deployed on a new chain or upgraded on existing one. Git push updates both contracts and submodules with contract artifacts, so UI and others repo knows all actual contract addresses. 
