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
run_unit_tests:
  before_script:
    - echo "First instruction"
  script:
    - echo "Running"
  after_script:
    - echo "Last instruction"
```
