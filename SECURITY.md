# Security Policy
The Solidity team and community take all security bugs in Solidity seriously.
We appreciate your efforts and responsible disclosure and will make every effort to acknowledge your contributions.

## Scope
Bugs in the Solidity repository are in scope.
Bugs in third-party dependencies e.g., jsoncpp, boost etc. are not in scope unless they result in a Solidity specific bug.

Only bugs that have a demonstrable security impact on smart contracts are in scope.
For example, a Solidity program whose optimization is incorrect (e.g., leads to an incorrect output) qualifies as a security bug.

## Supported Versions
As a general rule, only the latest release gets security updates.
Exceptions may be made when the current breaking release is relatively new, e.g. less than three months old.
If you are reporting a bug, please state clearly the Solidity version(s) it affects.

Example 1: Assuming the current release is `0.6.3` and a security bug has been found in it that affects both `0.5.x` and `0.6.x` trees, we may not only patch `0.6.3` (the bug-fix release numbered `0.6.4`) but `0.5.x` as well (the bug-fix release numbered `0.5.(x+1)`).

Example 2: Assuming the current release is `0.6.25` and a security bug has been found in it, we may only patch `0.6.25` (in the bug-fix release numbered `0.6.26`) even if the bug affects a previous tree such as `0.5.x`.

## Reporting a Vulnerability

To report a vulnerability, please follow the instructions stated in the doc.

In the bug report, please include all details necessary to reproduce the vulnerability such as:

- Input program that triggers the bug
- Compiler version affected
- Target EVM version
- Framework/IDE if applicable
- EVM execution environment/client if applicable
- Operating system
