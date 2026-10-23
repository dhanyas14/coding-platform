# Coding Platform

A browser-based coding challenge platform built with React and Node.js. It lets users solve algorithmic problems in multiple languages, run code against test cases, submit solutions, and evaluate outcomes through a Docker-backed sandboxed execution environment.

## Features

- Multi-language code editor for:
  - JavaScript
  - Python
  - C
  - C++
  - Java
- Problem-based challenge flow with prompts, constraints, and sample cases
- Run code against custom test cases
- Submit solutions and track score
- Docker-backed execution for safer sandboxed code evaluation
- Time and memory limits during execution
- Configurable frontend API base URL
- Anti-cheating safeguards such as fullscreen enforcement and copy/paste restrictions

## Tech Stack

- Frontend: React, Vite-style CRA setup, CodeMirror
- Backend: Node.js, Express
- Sandbox: Docker judge images
- Languages supported: JavaScript, Python, C, C++, Java

## Project Structure

```bash
.
├── public/
├── src/
│   ├── App.js
│   ├── App.css
│   └── ...
├── server/
│   ├── server.js
│   ├── executor.js
│   └── package.json
├── judge/
│   └── images/
│       ├── c/
│       ├── cpp/
│       ├── java/
│       └── node/
├── compiler/
├── docker-compose.yml
├── package.json
├── package-lock.json
├── README.md
├── SCHEMA.md
└── .gitignore
