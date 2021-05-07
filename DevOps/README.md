# DevOps & Continuous Testing (2020-2021)

## Teaching Staff

  * [Guilhem Molines](guilhem.molines@univ-cotedazur.fr), IBM France Lab, Université Côte d'Azur (co-head, DevOps)
  * [Salah Dahmoul](Salah.DAHMOUL@univ-cotedazur.fr), Sequoiasoft, Université Côte d'Azur (DevOps)
  * [Nikita Rousseau](TBD@univ-cotedazur.fr), Orange, Université Côte d'Azur (DevOps)


## Lecture Material

   * Week 1: [Devops Overview](https://github.com/collet/isa-devops/blob/master/DevOps/week1_overview_devops_v0.2.pdf)
   * Week 2: [Testing](https://github.com/collet/isa-devops/blob/master/DevOps/week2_testing_v0.4.pdf)
   * Week 3: [Continuous Integration](https://github.com/collet/isa-devops/blob/master/DevOps/week3_software_factory_v0.6.pdf)
   * Week 7: [Containers](https://github.com/collet/isa-devops/blob/master/DevOps/week7_containers_v0.6.pdf)
   * Week 8: [Deployment at scale](https://github.com/collet/isa-devops/blob/master/DevOps/week8_deployment_at_scale_v0.2.pdf)
   * Week 9: [Kubernetes](https://github.com/collet/isa-devops/blob/master/DevOps/week9_deployment_orchestration_v0.2.pdf)


## Deliverables

### Final Project Delivery (deadline: May 9th, 6pm)

You need to put in the README.md at the root of your main repository the distribution of points on each team member (100 points per member for a start)

 We will checkout your code in the main repository, with the git options to extract the tag final_deliverable and to follow sub-modules.
 
Once done, we will launch the script build.sh that you will have placed at the root of this extraction. This scripts should trigger a full build of everything all the way to the docker images of your project. Our evaluation machines have (at least) bash, maven, python, ant, perl, docker on them. Should anything else be required for the script to run, then the script has to say it.

Once the script finishes successfully, we will launch the script run.sh which you will have provided. This script is supposed to launch your project (database, dependents, server), most likely with a docker-composer up command.
Once this script finishes, we assume the server is up, we will then open the file scenarios.md placed at the root of your directory, which should guide us through what to do to run the scenarios. In a separate terminal, we will launch the script client.sh to launch the CLI client, and we will follow the scenarios described in the scenarios.md file to run through the demo ourselves.

Finally, we will launch the script jenkins.sh, which you should set up so that it launches a jenkins docker container pointing to a volume located in one of the sub-directories of your git repository, in which you will have copied the content of the volume you use as a data storage of your current jenkins. This way, we'll be able to point a browser at this jenkins instance and browse your build plans to check how they are setup. Be careful that if your volume contains the docker registry, it may end-up being too big, so strip it so that it only includes the build plans. Alternatively, if you have hosted Jenkins on the cloud, your jenkins.sh script should simply display the URL, user and password that we can use to browse it there
