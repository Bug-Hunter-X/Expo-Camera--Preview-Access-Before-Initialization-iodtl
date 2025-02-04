# Expo Camera: Preview Access Before Initialization

This repository demonstrates a common error encountered when using the Expo Camera API: attempting to access the camera preview before it's fully initialized.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides the corrected version.

## Problem

Accessing camera properties or starting recording too early after mounting the Camera component can lead to unexpected behavior such as undefined values or crashes. The `Camera.getStatusAsync()` method can mitigate this issue. 

## Solution

The solution uses `Camera.getStatusAsync()` to check the camera's status before accessing its preview or starting recording. This ensures the camera is properly initialized before accessing its functionality.

## How to run

1. Clone this repository.
2. Navigate to the directory using the command line.
3. Run `expo start` to begin the development server.
4. Observe the behavior and the improved functionality using the solution.