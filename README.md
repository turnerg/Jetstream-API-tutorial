# Jetstream-API-tutorial

A brief introduction to using command line clients to create, manipulate,
utilize, remove, and/or destroy OpenStack cyberinfrastructure.  

You will find two different 
versions of the tutorial in this repository.  
The two tutorials are identical with the exception of the naming convention 
of OpenStack entities.
The ClassRoom-Tutorial uses
the nomenclature <i>${OS_USERNAME}</i>-whatnot to name OpenStack entities and the General-Tutorial 
uses the nomenclature <i>${OS_PROJECT_NAME}-${OS_USERNAME}</i>-whatnot.  

Why is all of this important? OpenStack will let you create more than one entity with
the same name. When this occurs, you have to use the UUID (that long horrible string) 
instead of the easy to remember name. In the classroom setting, all the students
are in the same project and each has a unique username.  If they just use their
username, then there will be no name collisions.  In the general case, when looking 
at the big picture, user (and their username) could be in multiple projects. By pre-pending 
the project name, then the user can be assured they're looking at the correct entity
for the project they're working with.  Similarly, when ou have multiple users working 
in the same project, it is easy to identify entities that belong to the project and 
who created them.



One final note, one of the goals was that 
one could cut-&-paste the commands instead of fiddling with typing, the resulting typos, frustrations,
and falling behind in the tutorial.  This goal was met with the exception of one command that 
creates the IP address; the user will have to look at the output, grab the IP address, 
and enter it into the following associate command.





# ClassRoom-Tutorial.md

In a classroom setting, all the users are in the same OpenStack project and using
the OS_PROJECT_NAME is redundant, confusing, and causes unnecessary typing.  
The ClassRoom-Tutorial is also useful if you are the only user in a project; i.e. 
you won't be creating infrastructure that has the same name as a co-worker.


<a href="https://github.com/turnerg/Jetstream-API-tutorial/blob/master/ClassRoom-Tutorial.md">
ClassRoom-Tutorial</a> 


# General-Tutorial.md

The General-Tutorial is useful
in a setting where there are multiple users operating in one OpenStack project; this allows
your infrastructure to co-exist with your co-workers.  Again, this is meant mostly
in a learning environment; once you understand what's going on, you could create 
entities with meaningful names and share infrastructure. 
 

<a href="https://github.com/turnerg/Jetstream-API-tutorial/blob/master/General-Tutorial.md">
General-Tutorial</a> 


# Quickie Script

If you have used the General-Tutorial and left the network, keys, etc. in place, you 
can use this script to spin up a quick instance.  If you give no parameters, it'll
start an m1.tiny CentOS-7 instance. Output from the OpenStack commands are written 
to the screen as well as a file.  There is a final snippet you can cut-&-paste to
clean up everyting. 

<a href="https://github.com/turnerg/Jetstream-API-tutorial/blob/master/quickie-instance.sh">
quickie-instance.sh</a> 

### Parameter #1 is the name of the image to boot otherwise use the latest CentOS-7 image. 
You can use the generic names <b>centos</b> and <b>ubuntu</b> and it should pick up the 
lastest version of the requested image 


### Parameter #2 is the name to give the running instance; default is the image name with a random string appended


### Parameter #3 is the instance flavor to create; default is to make it a tiny
