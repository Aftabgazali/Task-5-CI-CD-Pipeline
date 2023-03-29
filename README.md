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


 ![image](https://user-images.githubusercontent.com/52740449/228616367-cea1a558-8511-4e23-8969-fa42f62cb886.png)
 
                                                                  Build Job
                                                                  
![image](https://user-images.githubusercontent.com/52740449/228616478-f384df80-5aae-4b7c-951a-c59f559b6e21.png)

                                                                    Failed Unit Test Job
                                                                   
                                                                         
![image](https://user-images.githubusercontent.com/52740449/228616641-6722377c-c404-4604-876d-6a6ba86cbc6a.png)

                                                                    Fixing Unit Test Job 
     
A Docker image build is the process of creating a Docker image from a Dockerfile. A Docker image is a lightweight, standalone, executable package that contains everything needed to run an application, including the code, runtime, libraries, and dependencies.

The Docker image build process starts with a Dockerfile, which is a text file that contains a set of instructions for building the image. The Dockerfile typically includes instructions for installing dependencies, copying files into the image, and setting configuration options.

When you run the docker build command, Docker reads the instructions in the Dockerfile and executes each instruction to create layers in the image. Each layer represents a step in the build process and contains only the changes made by that step. This allows Docker to reuse layers from previous builds, which can significantly speed up the build process.

Once the build process is complete, Docker creates an image that includes all of the layers. The resulting image can then be used to run containers, which are instances of the image that can be started and stopped as needed.

!![image](https://user-images.githubusercontent.com/52740449/228616772-aa9d5706-34be-47e6-a73b-8326cfe2374c.png)
                                                                       
                                                                       Docker Image Build
