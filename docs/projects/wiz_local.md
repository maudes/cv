---
title: WiZ Smart Lighting System
layout: blog
icon: material/dev-to
tags: [iot, python, streamlit, automation_test, cli_tool, pytest]
description: Developed a tool for anyone who'd like to test local control with their WiZ devices
---
![Image](/assets/images/wiz_smart_lighting.png)

## Project Overview

> Streamlining Smart Lighting Local Control Validation

As a Product Manager for WiZ's API services, I managed the end-to-end integration of smart lighting solutions, covering both cloud and local control protocols. My responsibilities included providing technical support to external partners, defining feature requirements, and facilitating integration processes. A recurring challenge during PoC (Proof-of-Concept) and partner validation was the absence of a lightweight, reliable tool for testing local command protocols, especially for developers aiming to build pure local controllers.

To address this critical gap, I independently designed and developed the WiZ Light Local Test Script. This Python-based CLI utility enables UDP-based local control testing. 


## Team & My Role
This was an independent development project that I undertook to solve a critical operational challenge within my product management role. I was solely responsible for the entire lifecycle: from identifying the problem and designing the solution to coding, testing, and refining the tool.


## Challenges

- Lack of lightweight tooling for validating local control commands during partner onboarding and PoC phases
- Need for a fast, reproducible way to test UDP-based local protocols and an example for reference


## Technical Stack

- **Language**: Python
- **Testing Framework**: Pytest
- **Interface**: CLI (Streamlit for an optional GUI)
- **Key Modules**: UDP communication, Test Runner, Device-Type Abstraction
- **Architecture**: Modular design with clear separation of concerns.

### What I Built & How

As the sole developer and owner of this project, my contributions spanned the entire development spectrum:

- **End-to-End Development**: Independently designed and implemented the entire Python-based CLI tool, enabling the sending of local control commands (e.g., turn on/off, change brightness) based on specific device types via UDP.

- **Rapid Validation Enablement**: Integrated functionality for quick validation of device responses using simple command-line inputs, enhancing testing efficiency.

- **Test Runner and Type Abstraction**: Developed the `runner.py` and `type_data.py` modules to manage test cases based on different device types, ensuring comprehensive and adaptable testing.

- **Modular Architecture Design**: Post-employment, I refactored the tool into a highly modular architecture, significantly improving its maintainability, extensibility, and reusability across various device types and testing scenarios. This design makes it ideal for PoC and QA environments.

- **Documentation & Examples**: Provided clear documentation and usage examples to streamline testing workflows for both internal teams and external partners.

**Project Structure**

```
 wiz-light-local-test-script
｜＿＿ modules/                  # For the use of cli.py and app.py 
｜    ｜＿＿ __init__.py      
｜    ｜＿＿ communication.py    # Build the udp connection, send and receive the udp packet
｜    ｜＿＿ runner.py           # Run the test cases
｜    ｜＿＿ type_data.py        # Test cases based on different device types
｜＿＿ pytest/ 
｜    ｜＿＿ tests/
｜    ｜   ｜＿＿ conftest.py
｜    ｜   ｜＿＿ test_basic.py
｜    ｜＿＿ pytest.ini
｜＿＿ simple_scripts
｜    ｜＿＿ basic_refactor.py
｜    ｜＿＿ basic.py
｜＿＿ cli.py                    # CLI tool
｜＿＿ app.py                    # streamlit
｜＿＿ README.md
```

> [GitHub project: Local Control Test Script for WiZ Lights](https://github.com/maudes/wiz-light-local-test-script)

## Software Development Life Cycle
As an independent project driven by a critical operational need, I followed an agile and iterative approach, prioritizing rapid delivery and continuous improvement.

### Initiation

- **Problem Identification**: Identified the recurring pain point during partner integrations: the lack of a reliable, cloud-independent tool for local control testing.
- **Solution Conceptualization**: Envisioned a lightweight Python-based CLI tool as the optimal solution to address this specific need.

### Planning

- **Technical Design**: Planned the core modules (UDP communication, test runner, device type abstraction) and determined the use of Python for its simplicity and robustness.
- **Feature Prioritization**: Focused on core functionalities like turning devices on/off and changing brightness first, with an eye towards future expansions.
- **Test Case Definition**: Outlined initial test cases based on common device behaviors and partner validation requirements.

### Development & Testing (Test-Driven Mindset)

- **Iterative Coding**: Developed the tool iteratively, building out the UDP communication layer, followed by the command parsing and test runner functionalities.
- **Testing Integration**: Used pytest to build automated tests, focusing on validating the correctness of UDP packet construction and device response parsing. This facilitated a test-driven mindset, ensuring the reliability of the commands sent.
- **Refinement Post-Employment**: After leaving WiZ, I dedicated time to refactor the entire codebase, transforming it into the current modular and maintainable structure. This significant refactor involved reorganizing modules, enhancing abstraction, and improving overall code quality.

### Release & Deployment

- **Share with the Community**
- **Documentation**: Created clear README.md documentation with usage examples to enable easy adoption by non-developers.

### Metric Review & Iteration

- **Continuous Improvement**: Based on usage and feedback, I continued to refine the script, notably through the post-employment refactoring, to ensure it remained a highly effective and adaptable tool for local control testing.


## Achievements

- **End-to-End Ownership & Impact**: Demonstrated full ownership from identifying a critical operational need to independently designing, building, and refining a practical solution. This tool directly improved users' understanding of local communication mechanisms and their limitations for WiZ smart lighting products, significantly streamlining technical support and clarifying protocol boundaries.

- **Modular Architecture Refinement**: Successfully refactored the entire tool into a highly modular and maintainable architecture, making it significantly easier to extend, reuse across different device types, and adapt for various testing scenarios. This refactoring greatly enhanced its long-term value.

- **Solving a Critical Business Problem**: Developed a lightweight, cloud-independent CLI utility that effectively addressed the challenge of validating local control commands, proving invaluable for PoC phases and ensuring reliable device behavior even without robust cloud connectivity.

**Note:** This project was developed for personal use during my tenure at WiZ and was not formally shared externally. Post-employment, I expanded and modularized it for broader applicability and maintainability.

<br>
