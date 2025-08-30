---
title: Carepilot Dashboard
layout: blog
icon: material/dev-to
tags: [python, streamlit, fastapi, sqlalchemy, pytest]
description: CarePilot is a personal project designed to help users record and track their health data over time. 
---
![Image](../assets/images/wiz_smart_lighting.png)

## Project Overview  

> Tagline

Main description

---

## Role & Scope  
Sole developer and product owner of the project. Led the full lifecycle from problem identification and technical design to implementation, testing, and post-employment refactoring.

---

## Key Challenges & Solutions  

- **Tooling Gap for Local Testing**：Built a lightweight, cloud-independent utility to validate local control commands during PoC and partner integration  
- **Protocol Complexity**：Abstracted device types and command flows to simplify UDP-based testing for developers  
- **Maintainability & Extensibility**：Refactored into a modular architecture post-employment to support broader use cases and long-term maintainability  

---

## Key Contributions & Impact  

- **End-to-End Development**：Built CLI tool with UDP communication, test runner, and device-type abstraction modules  
- **Test-Driven Approach**：Implemented pytest-based automated tests to ensure reliability and correctness of command execution  
- **Modular Architecture**：Refactored codebase into reusable modules for enhanced scalability across device types and testing scenarios  
- **Documentation & Enablement**：Provided clear usage examples and README to support internal and external adoption  
- **Operational Efficiency**：Streamlined partner validation workflows and clarified protocol boundaries for WiZ smart lighting products  

---

## Software Development Lifecycle  

| Phase                   | Key Activities                                                                 |
|-------------------------|--------------------------------------------------------------------------------|
| **Initiation**          | - Identified lack of local testing tools<br>- Proposed Python CLI solution |
| **Planning**            | - Designed core modules: UDP, runner, type abstraction<br>- Prioritized key features |
| **Development & Testing** | - Built iteratively with pytest integration<br>- Validated packet construction and device responses |
| **Release & Deployment** | - Published tool with documentation<br>- Refactored post-employment for modularity |
| **Iteration & Impact**   | - Continued refinement based on usage<br>- Improved adaptability for PoC and QA environments |


### Project Structure
The tool follows a modular architecture for maintainability and extensibility:

```
 wiz-light-local-test-script
｜＿＿ modules/                 
｜    ｜＿＿ __init__.py      
｜    ｜＿＿ communication.py    
｜    ｜＿＿ runner.py           
｜    ｜＿＿ type_data.py        # Test cases based on different device types
｜＿＿ pytest/ 
｜    ｜＿＿ tests/
｜    ｜   ｜＿＿ conftest.py
｜    ｜   ｜＿＿ test_basic.py
｜    ｜＿＿ pytest.ini
｜＿＿ simple_scripts
｜    ｜＿＿ basic_refactor.py
｜    ｜＿＿ basic.py
｜＿＿ cli.py                    # CLI entry point
｜＿＿ app.py                    # Optional Streamlit GUI
｜＿＿ README.md
```

**GitHub Repository**: [CarePilot Dashboard](https://github.com/maudes/carepilot-dashboard)

<br>
