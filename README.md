# CI-CD Pipeline
##  Create a CI-CD pipeline for a sample application using any CI-CD tool of your choice like Jenkins, Azure DevOps, Gitlab, Github Actions, AWS CodePipeline or any other tool of your choice. Include a code build and a docker build step in your pipeline.

We have used GitLab and a personal runner to do this task.

To build a job in a pipeline, you can follow these general steps:

Define your pipeline: A pipeline is a set of stages that define a series of steps that will be executed in order to build your job. You can define your pipeline in a file (e.g. Jenkinsfile) or through the web interface of your CI/CD tool.

Define your stages: A stage is a logical group of steps that have a specific purpose. For example, you may have a stage to build your code, a stage to run tests, and a stage to deploy your application. Each stage is defined using the 'stage' keyword, followed by the name of the stage.

Define your steps: Steps are the individual tasks that make up each stage. These can include things like checking out code from a repository, compiling code, running tests, and deploying to a target environment. Each step is defined using a specific keyword or plugin, depending on the CI/CD tool you are using.

Define your triggers: Triggers determine when your pipeline should run. These can include things like a commit to a specific branch, a new pull request, or a schedule.

Configure your pipeline: You may need to configure your pipeline to define variables, specify settings, or add plugins to extend the functionality of your pipeline.

Run your pipeline: Once your pipeline is defined, you can run it manually or configure it to run automatically whenever a trigger condition is met.

![Deploy job](https://user-images.githubusercontent.com/52740449/228614659-a169230c-6e1f-4481-bf85-80dfbab41852.png)
                                                                    
                                                                  Build Job
                                                                  
![Unit Test Job Failed](https://user-images.githubusercontent.com/52740449/228615589-407882f8-0e4c-42d8-9fcd-6a75b3828ad5.png)

                                                                    Failed Unit Test Job
                                                                   
                                                                         
![Unit Test Job Succeeded](https://user-images.githubusercontent.com/52740449/228615871-1b8b60c7-9b37-4d3b-9801-74a4b9344450.png)

                                                                    Fixing Unit Test Job 
     
     
![docker image build](https://user-images.githubusercontent.com/52740449/228616034-40933f90-5cbc-4e99-b8d6-6047de742e86.png)

                                                                        Docker Image Build
