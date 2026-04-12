---
name: unittest
version: 1.0.0
description: Define a unittest writing skill 
---

# When to use this skill

Use this skill when you want to create a angular unit test for project.

# Requirements
- list of class and method you need to cover
- list of usecases

# How to use it
1. Prepare test plan using @.agents/skills/unittest-testplan/SKILL.md skill. The test plan should include list of usecases and test cases for each usecase.
2. Create unit test using [unittest_class.md](./templates/unittest_class.md) template

# Rules
- Use ITestOutputHelper Output method BuildLoggerFor<Type>() to create logger
- Testing classes should be in sepparate mock folder. DON'T define them in the `{TestedClassName}_Test`
- Folders in `{Project}.Test` must be same as `{Project}`. And `{TestedClassName}_Test` must in same folder as `{TestedClassName}`
```
- Project
    - FolderA
        - ClassA.cs
- Project.Test
    - FolderA
        - ClassA_Test.cs
```
