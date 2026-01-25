---
title: "Task 08 — Build a Simple Shell"
date: 2025-11-08
description: "Basic Unix Shell using C"
tags: ["amfoss-anveshan"]
draft: false
---

Developed a basic Unix shell using C to understand how command-line interfaces work.

## What’s Done

* Built a basic Unix shell in C with a command prompt and input parsing.
* Executed external commands using fork(), execvp(), and waitpid().
* Implemented built-in commands: cd, exit, and jobs.
* Supported background execution using &.
* Tracked and displayed background process PIDs.
* Prevented zombie processes using SIGCHLD handling.

## What I Couldn't Do

* Handle Ctrl+C to display background jobs. (Instead i Implemented "jobs" command to do the same)
* Handle Ctrl+Z to suspend foreground processes.

## GitHub Link 

* [Simple-Shell](https://github.com/abxijth/amfoss-curriculum/tree/main/Task-08) 



