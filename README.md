# React Native Benchmarking Repository

This repository offers a standardized tool set for benchmarking React Native applications, aiming to enhance development efficiency and inclusivity.

## Table of Contents

- [Introduction](#react-native-benchmarking-repository)
- [Why Now?](#why-now)
- [Standardization](#standardization)
- [Test Suite](#test-suite)
- [Benchmarked Libraries](#benchmarked-libraries)
- [Getting Started](#getting-started)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Why now?

The React Native ecosystem needs a comprehensive and standardized benchmarking tool that reflects real-world scenarios and diverse hardware, leading to more effective and inclusive React Native development. The number of styling libraries have doubled in 2023, but each is using a different benchmark repo with different tests and different setups. The goal is to unify them under one roof and provide a clear picture for developers when deciding which one to use.

## Standardization

- Implement a comprehensive set of [tests](#test-suite) with varying complexity and performance is measured
- Integrates each [styled system](#styling-libraries) & [UI library](#ui-component-libraries)
- Ensure consistent styling approaches are used, such as inline styles vs. styled views
- Ensure a diverse range of devices that the community can test on and average out
- Use Production builds for measuring
- Present results benchmarked against the [GeekBench score](https://browser.geekbench.com/v6/cpu)

## Test suite

Styling systems libraries use Views, while UI component libraries use components.
Simulate re-rendering scenarios with 5 and 50 iterations to emulate real-world scenarios for low and high complexity applications.

1. Computation
  
    30x views / 1000x views

2. Re-rendering

    5 times / 50 times

### Future tests

3. Loading times
  
    first load vs warmed up load

4. Style complexity
  
    simple vs complex styles

5. Web performance & media queries


## Benchmarked libraries

If your library is not on any list PRs to include, integrate and benchmark them are open. Check the [Contributing](#contributing) section

### Styling libraries

Order based on the results from State of React Native 2023 [styling survey](https://results.stateofreactnative.com/styling/)

- [ ] [Unistyles](https://reactnativeunistyles.vercel.app/start/introduction/)

- [ ] [NativeWind](https://www.nativewind.dev/v4/overview)

- [ ] [Tamagui](https://tamagui.dev/docs/intro/introduction)

- [ ] [Restyle](https://shopify.github.io/restyle/)

- [ ] [gluestack-style](https://gluestack.io/style/docs/overview/introduction)

- [ ] [Dripsy](https://www.dripsy.xyz/)

### UI component libraries

Order based on the results from State of React Native 2023 [components survey](https://results.stateofreactnative.com/component-libraries/)

- [ ] [Tamagui](https://tamagui.dev/docs/intro/introduction)

- [ ] [gluestack-ui](https://gluestack.io/ui/docs/overview/introduction)

- [ ] [react-native-paper](https://callstack.github.io/react-native-paper/)

- [ ] [react-native-elements](https://reactnativeelements.com/docs)

- [ ] [react-native-ui-lib](https://wix.github.io/react-native-ui-lib/docs/getting-started/setup)

- [ ] [react-native-reusables](https://github.com/mrzachnugent/react-native-reusables)

## Getting Started

The project was started with [Expo](https://expo.dev), since this is the most popular React Native Framework.

`npx create-expo-app@latest --template tabs@50`

It is `bun` and `yarn` compatible.

Installing Dependencies

### yarn
```shell
yarn install
```
### bun
```shell
bun install --yarn #to generate yarn.lock
```

### Contributing

Contributions to the benchmarking repository are welcome! Whether you're a developer, tester, or enthusiast in the React Native community, your input can help shape and improve this tool. Please read our contributing guidelines for more information on how you can contribute.

### License

This project is licensed under the MIT License - see the [LICENSE.md](./LICENSE) file for details.

## Acknowledgments

Special thanks to [Nate](https://x.com/natebirdman) ([Tamagui](https://github.com/tamagui/tamagui)), [Marc](https://x.com/mrousavy) and [Hanno](https://x.com/hanno_jg) ([Margelo](https://github.com/margelo)), and [Jacek](https://x.com/jpudysz) ([Unistyles](https://github.com/jpudysz/react-native-unistyles)) for their help and support in reviewing the initial proposal and coming up with suggestions.

Thanks to all the contributors who have invested their time and effort in this project.