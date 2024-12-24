# Firebase Auth: Handling Invalid Email Addresses

This repository demonstrates a common but often overlooked issue in Firebase Authentication: unexpected errors caused by poorly formatted email addresses. The `bug.js` file shows how an invalid email can lead to a silent failure, while `bugSolution.js` provides a robust solution.

## Problem

The Firebase Authentication SDK doesn't always provide clear error messages when the email address used during signup or signin is invalid. This can result in frustrating debugging sessions, as the lack of an explicit error makes it hard to pinpoint the source of the problem.

## Solution

The solution involves implementing more rigorous email validation before interacting with the Firebase Authentication SDK. This preemptive check identifies invalid email formats early, providing a more user-friendly experience and simplifying debugging.

## Setup

1.  Ensure you have Node.js and npm installed.
2.  Install Firebase:
    ```bash
npm install firebase
    ```
3.  Configure your Firebase project (replace placeholders with your actual credentials).

## Usage

Run the `bug.js` and `bugSolution.js` files to see the problem and the improved solution in action.