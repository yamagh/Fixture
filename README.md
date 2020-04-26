# Fixture

<img src='icon/Fixture_Large.svg' width='250'/>

## What does this component do?

This component is a test fixture for OutSystems. This makes it easy to set up and tear down test data.

## ScreenShots

## Detailed description

Fixture will automatically create a test tenant using the multi-tenant mechanism.  
When you import the test data to the test tenant, input the test data to Fixture and it will be automatically imported.  
Use YAML because test data is easy to write and read.

Here is a sample.

```YAML
ToDoModule:
  ProjectEntity:
    MyProject:
      Id: &MyProject
      Name: Fixture
      Description: Test fixture for OutSystems.
  TodoEntity:
    Task1:
      ProjectId: *MyProject
      Title: Create module
      IsDone: False
    Task2:
      ProjectId: *MyProject
      Title: Create icon
      IsDone: True
```
