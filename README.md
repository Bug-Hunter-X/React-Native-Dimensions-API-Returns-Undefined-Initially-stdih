# React Native Dimensions API Returns Undefined Initially

This repository demonstrates a common issue in React Native where the `Dimensions` API returns `undefined` when accessing screen dimensions immediately after component mount or screen rotation.  The solution provides a robust method to handle this asynchronous behavior.

## Problem

The `Dimensions.get()` method might return `undefined` before the dimensions are ready, causing unexpected behavior or app crashes.  This is especially problematic in components that need these dimensions for layout or styling.

## Solution

The solution involves using the `Dimensions.addEventListener` to listen for changes in screen dimensions and setting the dimensions state accordingly, ensuring they're always defined.  This prevents the app from using `undefined` values before the dimensions are available.

## Usage

1. Clone the repository.
2. Navigate to the project directory.
3. Run `npm install` or `yarn install`.
4. Run the app using `react-native run-android` or `react-native run-ios`. 

Observe how the solution gracefully handles the initial `undefined` value and provides a smooth user experience.