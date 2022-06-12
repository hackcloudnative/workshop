# Basic Pipeline

## File name *.gitlab-ci.yml* 
### Simple Pipeline
```
run_tests:
  before_script:
    - echo "First started"
  script:
    - echo "Running"
  after_script:
    - echo "Last instruction"
```

# Pipelines with stages
```
stages:
  - first_stage
  - second_stage
  - third_stage
  
run_tests_1:
  stage: first_stage
  before_script:
    - echo "First instruction"
  script:
    - echo "Running"
  after_script:
    - echo "Last instruction"
    
run_tests2:
  stage: first_stage
  before_script:
    - echo "First instruction 2"
  script:
    - echo "Running 2"
  after_script:
    - echo "Last instruction 2"
```
