# Adapter

Adapter is a structural design pattern, which allows incompatible objects to collaborate.

4/4 star rating on [Refactoring Guru](https://refactoring.guru/design-patterns/adapter)

## Problem
You have some existing code that you want to reuse, but it has an incompatible interface. You want to use this code without modifying it.

## Solution
The Adapter pattern allows you to create a new class that wraps the existing code and provides a compatible interface. This new class is called the Adapter. The Adapter class implements the interface that the client expects and translates the calls to the existing code.

## Example

Let's say you have a `MediaPlayer` interface that has a method `play()`, and you have an existing class `AudioPlayer` that implements this interface. Now, you want to use a new class `VideoPlayer` that has a different interface with a method `playVideo()`. You can create an Adapter class `VideoPlayerAdapter` that implements the `MediaPlayer` interface and translates the calls to the `VideoPlayer` class.