# Assembler and Branch Predictor

Welcome to the Assembler and Branch Predictor repository. This project contains an assembler for converting assembly language code into machine code and a branch predictor for optimizing CPU performance by predicting the direction of branch instructions.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#Installation)
- [Usage](#Usage)
- [Contact](#contact)


## Introduction
The purpose of this project is to provide tools for assembling assembly code and predicting branch outcomes to enhance CPU performance. The assembler translates human-readable assembly language into machine code that can be executed by a processor. The branch predictor improves the execution speed of programs by guessing the outcome of branch instructions, reducing the number of CPU pipeline stalls.

## Features

1.RISC-V Assembler
-Supports a wide range of assembly instructions.
-Generates machine code for a specific target architecture.

2.Branch Predictor
-Implements common prediction algorithms (e.g. two-bit branch-prediction, one-bit, always-taken, always-nottaken).
-Evaluates prediction accuracy and performance.
-Configurable for different branch prediction strategies.

## Installation
-To get started with the project, clone the repository and install the necessary dependencies:
1.git clone https://github.com/Prathisthapandey12/RISC-V-Assembler-and-Branch-Predictor.git
2.cd RISC-V-Assembler-and-Branch-Predictor
3.Ensure you have C++ installed, and then install the required packages:

## Usage
Assembler
To assemble an assembly code file, use the following command:
g++ assembler.cpp
The output will be the corresponding machine code, saved to an output file.

Branch Predictor
To run the branch predictor on a set of branch instructions, use the following command:
g++ branch-prediction.cpp
You can specify different prediction strategies and evaluate their performance.

## Contact
Name: Prathistha Pandey
Github: Prathisthapandey12
