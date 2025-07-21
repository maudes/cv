---
title: WiZ Smart Lighting System
layout: blog
icon: material/home-automation
tags: [iot, python, streamlit, automation_test, cli_tool, pytest]
description: Developed a tool for anyone who'd like to test local control with their WiZ devices
---

## Project Overview

As the product manager for WiZ’s API services, I oversaw the full spectrum of smart lighting integrations, spanning both cloud and local control protocols. I worked closely with external partners to provide technical support, shape feature requirements, and align on certification processes. One recurring need during PoC and partner validation was a lightweight tool for testing local commands—without relying on cloud infrastructure.

While some community-developed tools exist—particularly from Home Assistant enthusiasts—I created a dedicated CLI utility for personal use: the WiZ Light Local Test Script. It’s a minimal yet effective solution for validating UDP-based local control commands, designed to streamline testing workflows and accelerate integration cycles.


## Challenges

- Lack of lightweight tooling for validating local control commands during partner onboarding and PoC phases
- Difficulty in controlling device behavior without good cloud connection (which happens a lot in demo stores)
- Need for a fast, reproducible way to test UDP-based local protocols and an example for reference

## Solutions

- Designed and implemented a Python-based CLI tool to send local control commands (e.g., turn on/off, change brightness) based on the device type via UDP
- Enabled quick validation of device responses using simple command-line inputs
- Provided clear documentation and usage examples to testing workflows

## Technical Stack

**#Python #pytest #streamlit**

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
｜＿＿ cli.py
｜＿＿ app.py                    # streamlit
｜＿＿ README.md
```

> [GitHub project: Local Control Test Script for WiZ Lights](https://github.com/maudes/wiz-light-local-test-script)

## Highlights

- Delivered a standalone tool with zero external dependencies—ideal for PoC and QA

<br>
