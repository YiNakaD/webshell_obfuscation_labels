
# RAWG WebShell Obfuscation Dataset

This repository contains an obfuscation-labeled WebShell corpus, used in our paper:

> **A Reward-driven Automated Webshell Malicious-code Generator for Red-teaming**  

## Overview

This dataset includes filenames of real-world WebShell samples along with their obfuscation category labels. Each file is mapped to one or more obfuscation types, annotated manually according to seven well-defined obfuscation strategies.

The goal of this dataset is to support research in adversarial code generation, malicious behavior understanding, and forensic analysis.

## File Description

- `webshell_obfuscation_labels.csv`:  
  A CSV file with the following format:
  
```

filename,category
.0byt3m1n1.php,"3,4,5"
0004b69af46f3eaa06710446e7a936e3.php,"1,3"
...

```

- `filename` refers to a PHP WebShell file from the original dataset.
- `category` contains a comma-separated list of obfuscation type IDs.

## Obfuscation Category Mapping

| ID | Description                                 |
|----|---------------------------------------------|
| 1  | Code Reordering / Unrelated Comments        |
| 2  | Functionally Equivalent Substitutions       |
| 3  | String Obfuscation / Encryption             |
| 4  | Code-Level Encryption / Obfuscation         |
| 5  | Dynamic Calls / Callbacks                   |
| 6  | Special Techniques                          |
| 7  | No Obfuscation                              |

## Source of Raw WebShell Files

The filenames in this dataset refer to samples from the open-source repository:

- **PHP-Webshell-Detection-via-Opcode-Analysis**  
GitHub: https://github.com/w-32768/PHP-Webshell-Detection-via-Opcode-Analysis

Please download the actual WebShell files from the above repository.
