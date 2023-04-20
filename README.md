#  Slither Detectors by Pessimistic.io

[![Blog](https://img.shields.io/badge/Blog-Link-blue?style=flat-square&logo=appveyor?logo=data:https://pessimistic.io/favicon.ico)](https://blog.pessimistic.io/)
[![Our Website](https://img.shields.io/badge/By-pessimistic.io-green?style=flat-square&logo=appveyor?logo=data:https://pessimistic.io/favicon.ico)](https://pessimistic.io/) 
[![Mail](https://img.shields.io/badge/Mail-gm%40pessimistic.io-orange?style=flat-square&logo=appveyor?logo=data:https://pessimistic.io/favicon.ico)](mailto:gm@pessimistic.io)

**Welcome!** We are the [pessimistic.io](https://pessimistic.io/) team, and in recent months we have been actively developing our [own **Slither detectors**](https://github.com/pessimistic-io/custom_detectors/tree/master/slither_pess/detectors) to help with code review and audit process. This repository contains everything you may require to work with them!

We increased the sensitivity of our detectors since they are *quite straightforward* and not written in the "original style." As a result, they produce FPs ([False Positives](https://en.wikipedia.org/wiki/False_positives_and_false_negatives)) more frequently than original ones. So that, our detectors are a kind of automation of the checks implemented in the checklist, their main purpose is to look for issues and assist the code auditor.

Please let us know if you have discovered an [issue/bug/vulnerability](https://telegra.ph/BountyCTF-Platforms-Web3-04-19) via our custom Slither detectors. You may contact us via opening a [PR/Issue](https://github.com/pessimistic-io/custom_detectors/issues) or [directly](mailto:gm@pessimistic.io), whichever is more convenient for you. If you have any further questions or suggestions, please [join our Discord Server](https://discord.gg/vPxkR8B9p7)! We hope to see you there, and we intend to support the community and its initiatives!

## Repository Navigation

#### **Table of Contents:**

| Section                      | Link                                                                                                          |
|------------------------------|---------------------------------------------------------------------------------------------------------------|
| Docs                         | [Docs for each detector](https://github.com/pessimistic-io/custom_detectors/tree/master/docs)                 |
| Slither_pess                 | [Detectors code](https://github.com/pessimistic-io/custom_detectors/tree/master/slither_pess)                 |
| Tests                        | [Test contracts for detectors](https://github.com/pessimistic-io/custom_detectors/tree/master/tests)          |
| Utils                        | [Auxiliary files](https://github.com/pessimistic-io/custom_detectors/tree/master/utils)                       |
| Issues                       | [Suggest an idea](https://github.com/pessimistic-io/custom_detectors/issues)                                  |
| Installation Process         | [Step-by-Step guide](https://github.com/pessimistic-io/custom_detectors#installation-process)                 |
| Detectors                    | [Detectors table](https://github.com/pessimistic-io/custom_detectors#detectors--table)                        |
| Enhancements & New Detectors | [Project Improvements](https://github.com/pessimistic-io/custom_detectors#enhancements--new-detectors)        |

## Installation Process

To install Pessimistic Detectors: 
1. Install the [original Slither](https://github.com/crytic/slither#how-to-install);
2. Clone our repository;
3. In our repository folder run:
```bash
python3 setup.py develop
```
> Keep in mind that you don't have to reinstall the plugin after changes in the repository!
4. To test the detectors on our test contracts, dependencies must be installed:
```bash
npm install
```

## **Detectors Table**

| Detector Link                                                                                                                                             | Docs & Setup                                                                                                     |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|
| [Unprotected Setter](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/unprotected_setter.py)                         | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/unprotected_setter.md)             |
| [Unprotected Initialize](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/unprotected_initialize.py)                 | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/unprotected_initialize.md)         |
| [TX Gasprice Warning](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/tx_gasprice_warning.py)                       | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/tx_gasprice_warning.md)            |
| [UniswapV2 Integration](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/uni_v2.py)                                  | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/integration_uniswapV2.md)          |
| [Token Fallback](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/token_fallback.py)                                 | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/token_fallback.md)                 |
| [Timelock Controller](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/timelock_controller.py)                       | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/timelock_controller.md)            |
| [Strange Setter](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/strange_setter.py)                                 | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/strange_setter.md)                 |
| [Read-only Reentrancy](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/read_only_reentrancy.py)                     | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/readonly_reentrancy.md)            |
| [NFT Approve Warning](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/nft_approve_warning.py)                       | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/nft_approve_warning.md)            |
| [Multiple Storage Read](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/multiple_storage_read.py)                   | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/multiple_storage_read.md)          |
| [Magic Number](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/magic_number.py)                                     | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/magic_number.md)                   |
| [Inconsistent Non-Reentrant](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/inconsistent_nonreentrant.py)          | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/inconsistent_nonreentrant.md)      |
| [Falsy Only EOA Modifier](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/falsy_only_eoa_modifier.py)               | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/falsy_only_eoa_modifier.md)        |
| [Missing Event Setter](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/event_setter.py)                             | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/event_setter.md)                   |
| [Dubious Typecast](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/dubious_typecast.py)                             | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/dubious_typecast.md)               |
| [Double Entry Token Possibility](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/double_entry_token_possibility.py) | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/double_entry_token_possibility.md) |
| [Call Forward To Protected](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/call_forward_to_protected.py)           | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/call_forward_to_protected.md)      |
| [Before Token Transfer](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/before_token_transfer.py)                   | [Explore](https://github.com/pessimistic-io/custom_detectors/blob/master/docs/before_token_transfer.md)          |

> Please note: there is one detector that is disabled by default: [pess-uni-v2](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/uni_v2.py). **It is recommended to run it only on projects that integrate [Uniswap V2](https://betterprogramming.pub/uniswap-v2-in-depth-98075c826254)!**

## Enhancements & New Detectors

Here we indicate our updates, workflows and mark completed tasks and improvements.

You can add your *detector/idea/enhancement* by [opening the Issue at the following link](https://github.com/pessimistic-io/custom_detectors/issues)!

If you want to add a *detector* make sure that:
1. Your detector is well described in a documentation file;
2. Detector test contract is present and compiles;
3. Detector code is present and works correctly;

If you want to add an *idea* make sure that:
1. Your idea is well described;
2. Vulnerability example is present;

If you want to add an *enhancement* make sure that:
1. Your enhancement does not worsen the base code;
2. Your enhancement is commented;

#### **Detectors Backlog:**

[![Issues](https://img.shields.io/github/issues/pessimistic-io/custom_detectors?style=flat-square)](https://github.com/pessimistic-io/custom_detectors/issues)
[![Open Pool Requests](https://img.shields.io/github/issues-pr/pessimistic-io/custom_detectors?style=flat-square)](https://github.com/pessimistic-io/custom_detectors/pulls)
[![Closed Pool Requests](https://img.shields.io/github/issues-pr-closed-raw/pessimistic-io/custom_detectors?style=flat-square)](https://github.com/pessimistic-io/custom_detectors/pulls?q=is%3Apr+is%3Aclosed)

| Task                                                                                                                                  | Status     |
|---------------------------------------------------------------------------------------------------------------------------------------|------------|
| Opensource current repository                                                                                                         | In Process |
| Fix - Readonly Reentrancy Detector                                                                                                    | Completed  |
| Suggestion - Write a Walkthrough Article                                                                                              | In Process |
| Add [UniswapV2 Integration](https://github.com/pessimistic-io/custom_detectors/blob/master/slither_pess/detectors/uni_v2.py) Detector | Completed  |

## Articles:

- [Slither: In-Depth](https://medium.com/coinmonks/slither-smart-contract-security-tools-29918df0fa8c)
- [Slither Review](https://blog.trailofbits.com/2019/05/27/slither-the-leading-static-analyzer-for-smart-contracts/)
- [Slither usage at Pessimistic](https://blog.pessimistic.io/slither-an-auditors-cornucopia-a8793ea96e67)

#

### We would also like to invite you to [visit our blog](https://blog.pessimistic.io/)!
### **We hope you find our work useful; we would appreciate any feedback, so please do not hesitate to [contact us](mailto:gm@pessimistic.io)!**
