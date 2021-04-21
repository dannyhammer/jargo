# Jargo

A simplified way of managing Java projects

## Table of Contents

- [Overview](#overview)
  - [Background](#background)
  - [Benefits](#benefits)
- [Usage](#usage)
- [Installing](#installing)

## Overview

Jargo is a simple project manager for Java, heavily inspired by Rust's [cargo](https://github.com/rust-lang/cargo/).

### Background

The idea for Jargo came from my dislike of having to use `javac` and `java` repeatedly while working with Java projects on the command line.
After I began using Rust, I saw the benefits of a proper package manager, so I looked to Maven and Gradle to handle similar functionality in Java.
Both of those options provided far more features and complexity than I needed, so I took matters into my own hands.
What originally began as two aliases in my shell's configuration file grew rapidly into Jargo.

Note: Jargo is not intended to be a replacement for Maven or Gradle, by any means.
This was created to make my life easier when working with Java on the command line, that's all.

### Features

I wanted Jargo to make project management simple, so I made sure it had the essentials:

- Create a new Java project
- Compile the project if source files have been edited
- Run the project in a one simple command

As I continued to write this, I discovered a few more features that were quite simple to implement and made the whole program feel a bit nicer, so I threw them in.

## Usage

The basic syntax is `jargo [OPTIONS] [COMMANDS]`, which is quite similar to `cargo` (for good reason).

Here are a few of the basic commands and options:

- `jargo new <PROJECT> [OPTIONS]` - Create and initialize a new Java project
- `jargo build` - Compile the current project
- `jargo run [ARGUMENTS]` - Execute the project with the supplied arguments, compiling if necessary
- `jargo clean` - Removes all `*.class` files
- `jargo doc` - Generate Javadocs for the current project

## Installation

Currently, cloning this repository is the only bit of installation necessary.
Of course, you need Java installed.

I'll put more in this section once I have this more fleshed out.
