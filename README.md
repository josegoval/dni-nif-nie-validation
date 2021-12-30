# nif-dni-nie-cif-validation

`nif-dni-nie-cif-validation` is a JS and TS library that makees everything related
with NIF (spanish identifiers) easier.

**Feel like supporting this free plugin?**

<a href="https://www.buymeacoffee.com/josegoval" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

**Table of Contents**

- [Installation](#installation)
- [Main Functions](#main-functions)
- [Other utilities](#other-utilities)

## Installation

```bash
npm install --save nif-dni-nie-cif-validation
```

or

```bash
yarn add nif-dni-nie-cif-validation
```

## Main functions

| Function                  | Description                                                                                                                                           | Expected inputs                               | Valid examples                      |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------- | ----------------------------------- |
| `isValidNif`              | Checks if the given nif (legal entity NIF or natural person NIF (DNI, DNI K, DNI L, DNI M, or NIE)) is valid.                                         | TODO                                          | TODO                                |
| `isValidNaturalPersonNif` | Checks if the given naturalPersonNif is whether a valid DNI (including DNI K, L and M) or a valid NIE.                                                | TODO                                          | TODO                                |
| `isValidDniLetter`        | Checks if the dni control code (letter) provided is valid. It does include checks for DNI K, L and M. _(WARNING!:It does not check the `DNI_REGEX`.)_ | `/^[KLM\d]{8}[TRWAGMYFPDXBNJZSQVHLCKE]$/i`    | `57655929N` `K0867756N`             |
| `isValidDni`              | Checks if the given dni is valid. It does include checks for DNI K, L and M.                                                                          | `/^[KLM\d]{8}[TRWAGMYFPDXBNJZSQVHLCKE]$/i`    | `57655929N` `K0867756N`             |
| `isValidNie`              | Checks if the given nie is valid.                                                                                                                     | `/^[XYZ][\d]{7}[TRWAGMYFPDXBNJZSQVHLCKET]$/i` | `Z9332057L` `X9864761S` `Y2541026T` |
| `replaceNieLetter`        | Returns a new string with the nie letter (XYZ) replaced. However it will throw an error if the first character is not X, Y or Z.valid.                | `/^[XYZ][\d]{7}[TRWAGMYFPDXBNJZSQVHLCKET]$/i` | `Z9332057L` `X9864761S` `Y2541026T` |

<!-- isValidLegalEntityNifControlCode -->

## Utility functions

## Other utilities

| Function                  | Description                                                                                                   | Allowed inputs | Valid examples |
| ------------------------- | ------------------------------------------------------------------------------------------------------------- | -------------- | -------------- |
| `isValidNif`              | Checks if the given nif (legal entity NIF or natural person NIF (DNI, DNI K, DNI L, DNI M, or NIE)) is valid. | TODO           | TODO           |
| `isValidNaturalPersonNif` | Checks if the given naturalPersonNif is whether a valid DNI (including DNI K, L and M) or a valid NIE.        | TODO           | TODO           |

https://es.wikipedia.org/wiki/N%C3%BAmero_de_identificaci%C3%B3n_fiscal

- [OK] isValidLegalEntityNif
- [OK] isValidNifK
- [OK] isValidNifL
- [OK] isValidNifM
- [OK] isValidLegalEntityNif more keys like old CIF?
  except LKM
- upload to npm
- README.me
- buy me a coffe
