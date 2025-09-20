# 🧵 User-Level Threads Library

## Overview
This project implements a static library in C++ for managing user-level threads with a customizable API. It provides thread creation, scheduling, blocking, and termination without relying on kernel threads, enabling efficient, lightweight concurrency.

## Features
- Thread lifecycle management: create, run, block, resume, terminate.
- Round-Robin scheduling with a configurable quantum.
- Signal-safe manipulation for thread switching and synchronization.
- Unique thread IDs allocation with recycling of freed IDs.
- Support for main thread and multiple user threads.
- Robust error handling and system call failure reporting.

## Skills & Concepts
- C++ programming with low-level system interaction.
- Use of `sigsetjmp` and `siglongjmp` for context switching.
- Signal handling and masking for race condition prevention.
- Implementation of Round-Robin Scheduler.
- Data structures for thread state management (queues, lists).
- Writing static libraries and well-documented APIs.

## Running & Testing
1. Compile the static library using the provided Makefile.
2. Link the library in user programs for threading functionality.
3. Use the `uthreads.h` interface following documented API functions.
4. Develop and run test programs to verify thread scheduling and behavior.

## Theory Questions
- Usage and behavior of `sigsetjmp` / `siglongjmp`.
- Advantages of user-level threads.
- Differences between processes and kernel threads.
- Signal handling in UNIX-like systems.
- Concepts of real vs virtual time in scheduling.
