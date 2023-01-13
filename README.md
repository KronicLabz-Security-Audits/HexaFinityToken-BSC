# HexaFinityToken-BSC

[![MythXBadge](https://badgen.net/https/api.mythx.io/v1/projects/dc75cd1c-38ed-4064-85d6-8737936adb8a/badge/data?cache=300&icon=https://raw.githubusercontent.com/ConsenSys/mythx-github-badge/main/logo_white.svg)](https://docs.mythx.io/dashboard/github-badges)



## SWC-108: State Variable Default Visibility
State variable visibility is not set.
It is best practice to set the visibility of state variables explicitly. The default visibility for "inSwapAndLiquify" is internal. Other possible visibility settings are public and private.

### Severity: Low

### Code
```
12 |          function decimals() external pure returns (uint8);
13 |      
14 |          function totalSupply() external view returns (uint256);
15 |      
16 |  >>>     function balanceOf(address owner) external view returns (uint256); <<<
```
        
