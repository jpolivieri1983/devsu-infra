# Infrastructure creation for Devsu Practical Assessment

In this repo you can find:
## Infrastructure definition
- Cloudformation yaml file (main-devsu.yml) with resources definition, including the ECS cluster which will execute the docker image from the practical assessment.

### Remarks:
    - Minimum amount of containers running: 2
    - Maximum amount of containers running: 4
    - Desired amount of containers running: 2 
    - Auto Scaling configured at 80% of average cpu utilization.


## Infrastructure Pipeline
- Workflow yaml file (.github/workflows/deploy-to-ecs.yml) to automatize the infrastructure creation using a GitHub Actions pipeline.

### Remarks:
    - Excution of Cloudformation template on a GitHub Actions workflow.
    - Access keys configured as secrets on GitHub Actions.
    - Values received as parameters to be reutilized on different environments.
  
