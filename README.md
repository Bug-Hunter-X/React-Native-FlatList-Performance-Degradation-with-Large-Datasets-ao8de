# React Native FlatList Performance Issue

This repository demonstrates a common performance problem encountered when using the `FlatList` component in React Native with a large dataset.  The provided code showcases the issue and a solution to improve rendering efficiency and prevent performance degradation.

## Problem

When rendering a large number of items in a `FlatList`, React Native can experience significant performance slowdowns. Scrolling becomes sluggish, frame drops occur, and in extreme cases, the app might crash.  The root cause often lies in inefficient rendering and unnecessary re-renders.

## Solution

The solution focuses on optimizing the rendering process through the use of techniques like `keyExtractor` to uniquely identify items, `ItemSeparatorComponent` to improve visual separation of items, and efficient data handling to minimize unnecessary re-renders.  The `renderItem` function should also be optimized to avoid expensive calculations within the rendering loop.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npx react-native run-android` or `npx react-native run-ios` to run the app.
4. Observe the performance when scrolling through the list of items.