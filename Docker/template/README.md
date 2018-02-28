# Guidelines for containerization at QBIC

First of all, please follow the template that can be found in this directory. Next, please follow this list of points to get what you want:


- Try to use a container from biocontainers - for many tools there is a pre-packaged version available, we don't need to reinvent the wheel. 
  - If there is a container, just import it in the template, add your name and the ENV variable and you're good.
  - If you need to add more, you may do so but please document in the Dockerfile what you did and WHY.
- Place at a minimum *two* Dockerfiles in the corresponding folder:
  - one in a separate versionized directory, following this standard: vX.Y.Z.U.V (where V denotes the version)
  - One in the topmost directory, containing the identical content as in the latest versionized directory folder

For an example, please look at the `Docker/fastqc/` folder. 

