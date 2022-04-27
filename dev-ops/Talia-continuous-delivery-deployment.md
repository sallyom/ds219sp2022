Describe the difference between Continuous Delivery and Continuous Deployment 

Continuous Delivery automatically deploys all code changes to a testing and/or production environment after the build stage. 
- relies on continuous integration
- Deployments need to be automated
- can release more often
With Continuous Depoloyment, every change that passes all stages of the production pipeline is released to the customers. There's no human intervention, and only a failed test will prevent a new change to be deployed to production.
- quality of test suite will determine the quality of releases
- develop faster as there's no need to pause development for releases
- releases are less risky and easier to fix in case of problem as you deploy small batches of changes
- Customers see a continuous stream of improvements, and quality increases every day
