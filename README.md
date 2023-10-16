# Infrastructure creation for Devsu Practical Assessment

In this repo you can find:
- Cloudformation yaml file (main-devsu.yml) with resources definition, including the ECS cluster which will execute the docker image from the practical assessment.
    Remarks:
    - Minimum amount of containers running: 2
    - Maximum amount of containers running: 4
    - Desired amount of containers running: 2 
    - Auto Scaling configured at 80% of average cpu utilization.

- Workflow yaml file (deploy-to-ecs.yml) to automatize the infrastructure creation using a GitHub Actions pipeline.

  
