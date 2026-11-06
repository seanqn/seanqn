## Hi there 👋

My github currently holds all of my projects; academic, personal, and otherwise. 3rd year CS student at Oklahoma State University. Looking to help build and support others driving their own solutions.

## Overview
### SimpleVault
<img width="695" height="595" alt="Screenshot 2026-11-05 at 7 05 13 PM" src="https://github.com/user-attachments/assets/995d729c-d34d-48e0-8bb1-e10805e79d9a" />

&nbsp;

Brief: SimpleVault is an in-development project that intends to store passwords, keys, phrases, and other credentials in a secure, local desktop application.
SimpleVault was first developed in Flutter using Dart before moving to Qt to improve C++ skills. The bulk of the current iteration of the project is a result of Qt development.
Here are a few features of the Qt/C++ version of SimpleVault:
- Foundation for authentication flow, generating and designating a UUID for a newly registered user, functions for account creation/deletion, states for user registration status
- Sign-in using MacOS device credential (utilizes qtkeychain as a keychain wrapper)
- Group management, allowing add/rename/removal of a 'group' holding credential entries
- Credential entry management; leverages a custom edit cache service that temporarily holds editing fields, updating database on focus loss/edit state change
- Cryptography service that depends on libsodium and emphasizes zeroing
- Local SQlite3 database
- Foundation for frontend

#### Migration
The project is currently being migrated to Rust/Node + Tauri for improved cross-platform interop and removing current framework dependencies

<img width="432" height="512" alt="Screenshot 2026-11-05 at 7 06 24 PM" src="https://github.com/user-attachments/assets/42e135e5-0f0d-4a2d-b991-e58566624dea" />

https://github.com/user-attachments/assets/66a71a8a-4afa-45a5-a4a4-58bbcc60196e

&nbsp;

### Pincer
Brief: Pincer is anticipated observability tool and debugger that would function like a playback tool for LLM processes. This is in early development and only supports OpenAI adapters at the moment.
Features:
- Terminal-based trace viewer that outputs relative trace information
- Prototype of the debugger that beautifies and displays trace information

&nbsp;

Example debugger output:
```
PINCER DEBUGGER — offline trace
Mode: inspection only | Execution control: unavailable

STEP  TYPE    NAME                RECORDED RESULT
01    model   synthetic-model     Ended; no reported error
02    tool    lookup              Ended; no reported error
03    tool    deliberate_failure  Error reported

Selected: Step 02 — lookup
Parent: demo
Start/end: recorded
Input: omitted from trace
Output: omitted from trace

Checkpoint assessment:
  Completed boundary: yes
  Resumable state saved: no

Commands: list | select <step> | details | next | previous | quit
```

&nbsp;
  
### Academic Projects
Several repos showcase some custom Abstract Data Types, ADT optimizers, and algorithms implemented into a subset of these. A few are:
- Binary Search Tree Validator: Validates whether a BT search was correct
- AVL Tree Nth Largest: Searches an AVL (Adelson-Velsky Landis) Tree with self-rotating behavior and tracks the largest node value
- List/Matrix Graph: ADT for each; list uses a linked behavior and matrix a 2D array for directed graph traversal
