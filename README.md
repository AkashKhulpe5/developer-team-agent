# Multi Agent QA Engineering System

Developer | Review (all the stds are met, syntax is correct, best practices are followed) | QA agent (ensures the quality of the output, test all the edge cases) | - Test cases are written for all new features | - Edge cases are identified and tested | - Performance is tested and optimized Fix agent (fixes any issues found during the review and QA process) | - Bugs are fixed | - Code is refactored for better readability and maintainability | - Performance is improved based on QA feedback Final report (summarizes the entire process, outcomes, and any follow-up actions)

Real engineering workflow involves:

Developers
Reviewers
Testers
Fixers/Developers
Architecture for the project
    User requirements (what the user wants to achieve)
            |
            V
    Developer agent (translates user requirements into code)
            |
            V
    (a)Review agent (reviews the code for correctness, style, and best practices)
            |
            V
    QA agent (ensures the quality of the output, test all the edge cases)
    Decision making (LOGIC written in graph and conditional edges)
    /             \
   V               V
Fix             Final report
|                   |
V                   V
Review agent(a) END

Nodes:
Developer Node
Review Node
QA Node
Fix Node
Final Report Node
State:
User requirements: str
Generated code: str
Review feedback: str
QA feedback: str
needs_fix: routing agent/decision: Bool
final report: str
iteration_count: int
Decision making of the routing agent is based on Router function (Logic) and the condition_edge (routing mechanism).


An intelligent agent based software engineering workflow where multiple AI agents collaborate to develop, review, test, fix, and validate code before final delivery.

This project mimics a real engineering pipeline used in software teams by combining autonomous agents with graph based decision routing.

## Features

- Requirement-to-code generation  
- Automated code review and best practice validation  
- Edge case testing and QA verification  
- Bug fixing and code optimization  
- Conditional routing based on quality checks  
- Final engineering report generation  


## Real Engineering Workflow

User Requirements  
↓  

Developer Agent  
↓  

Review Agent  
↓  

QA Agent  
↓  

Decision Routing  

If issues found → Fix Agent → Review Again  

If passed → Final Report → END  


## Architecture

User Requirements

        |
        
        V
        
Developer Agent

        |
        
        V
        
Review Agent

        |
        
        V
        
QA Agent
        |
        
        V
        
 Routing Logic
 
   /        \
   
  V          V
  
Fix Agent   Final Report

  |
  
  V
  
Review Agent

  |
  
 END

## Run

---bash 

## Create env

uv venv

--activate it

uv pip install -r requirements.txt

---bash

python main.py
