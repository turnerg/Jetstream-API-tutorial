# Jetstream-API-tutorial

A brief introduction to using command line clients to create, manipulate,
utilize, remove, and destroy OpenStack cyberinfrastructure.  

You will find two different 
versions in this repository.  
The two tutorials are the identical with the exception of the naming convention 
of OpenStack entities.
The ClassRoom tutorial uses
the nomenclature ${OS_USERNAME}-whatnot to name OpenStack entities and the General tutorial 
uses the nomenclature ${OS_PROJECT_NAME}-${OS_USERNAME}-whatnot



In a classroom setting, all the users are in the same OpenStack project and using
the OS_PROJECT_NAME is redundant, confusing, and causes unnecessary typing.  

The General-Tutorial is useful
in a setting where there are multiple users operating in one OpenStack project. 
If you are the only user in a project, or good at coordinating with your co-workers, 
the ClassRoom-Tutorial would work fine.  Again, the two tutorials are (meant to be) 
identical.  The General further 

# ClassRoom-Tutorial.md

<a href="https://github.com/turnerg/Jetstream-API-tutorial/blob/master/ClassRoom-Tutorial.md">
ClassRoom-Tutorial</a> 


# General-Tutorial.md


<a href="https://github.com/turnerg/Jetstream-API-tutorial/blob/master/General-Tutorial.md">
General-Tutorial</a> 


# Quickie Script

If you have used the General-Tutorial and left the network, keys, etc. in place, you 
can use this script to spin up a quick instance.
<a href="https://github.com/turnerg/Jetstream-API-tutorial/blob/master/quickie-instance.sh">
quickie-instance.sh</a> 

### Parameter #1 is the name of the image to boot otherwise use the latest CentOS-7 image
### Parameter #2 is the name to give the running instance; default is the image name with a random string appended
### PArameter #3 is the instance flavor to create; default is to make it a tiny
