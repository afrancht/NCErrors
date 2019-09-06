# Nucypher Error Report 1

## System Information

- MacOS Mojave 10.14.6 (18G95)
- MacBook Pro (13-inch, 2016, Four Thunderbolt 3 Ports)
- 2.9 GHz Intel Core i5
- 8 GB 2133 MHz LPDDR3

## Error 1 found in Installation Guide > Standard Pip Installation

- URL: https://docs.nucypher.com/en/latest/guides/installation_guide.html
- Video: https://youtu.be/XlOgVl2nfcI

When executing command 2: `$ (nucypher-venv) pip install -U nucypher`

It returns the following error:

'ERROR: Could not find a version that satisfies the requirement eth-account==0.4.0 (from nucypher) (from versions: 0.1.0a1, 0.1.0a2, 0.2.0a0, 0.2.0, 0.2.1, 0.2.2, 0.2.3, 0.3.0)
ERROR: No matching distribution found for eth-account==0.4.0 (from nucypher)'

Possible fix:
`$ pip install -U eth-tester`
