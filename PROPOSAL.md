# Proposal for Standardized React Native Benchmark Repository

This proposal aims to create a comprehensive and standardized benchmarking tool that reflects real-world scenarios and diverse hardware, leading to more effective and inclusive React Native development.
It is currently open to suggestions, discussions, and updates. All stakeholders should agree upon key aspects in order to guarantee a successful project.

## Objective:

Develop a standardized repository for benchmarking React Native applications, addressing key issues in the current benchmarking landscape.

## Key Points:

### 1. Standardization of Benchmarks:

- Establish a public repo that open source maintainers will use to test, develop and improve further their libraries
- Agree on a range of tests with varying complexity and performance is measured
- Ensure consistency in styling approaches, such as inline styles vs. styled views
- Ensure a diverse range of devices that the community can test on and average out
- Use Production builds for measuring

### 2. Test suite

The following test suite are implemented for styling systems, but also UI component libraries.

Styling systems will use Views, while UI components will use Buttons and common components.

Besides view computation, re-renders are included to emulate real-world scenarios for low and high complexity applications.

- 30x computation
- 1000x computation
- re-rendering 5x
- re-rendering 50x

### 3. Roadmap

- Use de-facto popular tools to create the project, i.e. [Expo](https://expo.dev/)
- Prepare a tab for each test suite (comp 30x, comp 1000x, rr 5x, rr 50x)
- Each creator integrates their library as they know best
- Run tests on physical devices, not simulators

### 4. Nice to haves

- Web benchmarks
