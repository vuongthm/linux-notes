---
id: "field-notes:linux-terminal-first-steps"
translationKey: "field-notes:linux-terminal-first-steps"
title: "Linux: first steps in the terminal — sample lab"
description: "A sample exercise in finding your location, listing files, and observing a system before changing it."
topics: ["linux"]
tags: ["linux", "terminal"]
date: "2026-11-04"
kind: "lab"
level: "beginner"
---

> This is sample library content. Replace it with your own notes and observations.

## Find your location

Open a Linux terminal and run each command separately. This exercise does not require administrator privileges.

```sh
whoami
pwd
ls -la
```

`whoami` shows the current username. `pwd` prints the working directory. `ls -la` includes hidden entries and detailed file information. Observe your actual output rather than comparing it with invented example results.

## Use a separate practice directory

Create a directory inside your home directory and enter it:

```sh
mkdir -p ~/terminal-practice
cd ~/terminal-practice
pwd
```

The shell expands `~` to your home directory. `cd` changes the working directory; use `cd ..` to move to its parent.

## Observe before editing

```sh
uname -a
```

This displays kernel and system information. It does not replace distribution-version information. A hostname may appear in the output; review it before sharing terminal screenshots.

## Write down what you learned

- Which directory does a new terminal start in?
- How are filenames beginning with a dot displayed?
- How does `pwd` change after `cd ..`?

Answer in your own words, with your operating system and exercise date, to turn this sample into personal notes.

```quiz
{
  "title": "Check your understanding",
  "questions": [
    {
      "id": "q1",
      "question": "Which command prints the current working directory?",
      "options": [
        "uname -a",
        "pwd",
        "whoami"
      ],
      "answer": 1,
      "explanation": "pwd reports the current directory; whoami reports the user and uname reports system/kernel information."
    },
    {
      "id": "q2",
      "question": "What does -a add to ls -la?",
      "options": [
        "Automatic movement to the parent directory",
        "Entries whose names begin with a dot",
        "Only audio files"
      ],
      "answer": 1,
      "explanation": "ls -a includes dot-prefixed entries; cd .. changes to the parent directory."
    }
  ]
}
```
