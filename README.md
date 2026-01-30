# Thread Hijacking Proof of Concept

## DISCLAIMER
**FOR EDUCATIONAL AND RESEARCH PURPOSES ONLY**

This repository contains proof-of-concept code demonstrating thread hijacking techniques.
Only use on systems you own or have explicit permission to test.

## Description
Demonstration of remote thread hijacking using CreateRemoteThread with CREATE_SUSPENDED flag.
The technique involves creating a suspended remote thread and redirecting its execution
by modifying the instruction pointer (RIP/EIP).

## Features
- Remote thread creation in suspended state
- Thread context manipulation
- Instruction pointer redirection
- Shellcode execution in target process
- Clean state restoration (conceptual)

# Usage
thread_hijack.exe [target_pid]

# Test with provided example
g++ -o test_target examples/test_target.cpp
./test_target &  # Get its PID
./thread_hijack.exe [pid]
