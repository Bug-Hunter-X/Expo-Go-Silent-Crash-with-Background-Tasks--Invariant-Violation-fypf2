# Expo Go Silent Crash with Background Tasks

This repository demonstrates a bug where an Expo app using background tasks crashes silently in Expo Go, showing only an `Invariant Violation: Native module cannot be null` error in the console.  The issue stems from improper registration or definition of the background task within the Expo TaskManager API.

## Reproduction

1. Clone this repository.
2. Run `npm install`.
3. Open the project in Expo Go.
4. Observe the silent crash.  Check the console for the error message.

## Solution

The solution involves ensuring the background task is correctly registered and defined. The corrected code is provided in `backgroundTaskSolution.js`.

## Additional Notes

This bug can be challenging to debug due to the lack of a clear error message within the Expo Go app.  Thoroughly checking the `TaskManager` setup and the background task function definition is crucial for resolving this issue.