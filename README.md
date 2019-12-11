Virtualisation
---

A virtual machine is a computer file, typically called an image, that behaves like an actual computer. In other words, a computer is created within a computer. It runs in a window, much like any other program, giving the end user the same experience on a virtual machine as they would have on the host operating system itself. The virtual machine is sandboxed from the rest of the system, meaning that the software inside a virtual machine can’t escape or tamper with the computer itself. This produces an ideal environment for testing other operating systems including beta releases, accessing virus-infected data, creating operating system backups and running software or applications on operating systems they weren’t originally intended for.

Virtualization technology has serious drawbacks, such as performance degradation due to the heavyweight nature of virtual machines(VM), the lack of application portability, slowness in provisioning of IT resources



A Docker container is a software bucket comprising everything necessary to run the software independently. There can be multiple Docker containers in a single machine and containers are completely isolated from one another as well as from the host machine.

So essentially the main difference between virtualisation and containerisation is that with containers everything is faster and more lightweight. This is because when you are creating a virtual machine, you need to create a guest OS and have an underlying hypervisor to orchestrate all the guest OS’s on the hardware. However with containers, you are essentially reducing this down to just having the software bucket without the need for a guest OS meaning that it is far more lightweight.

Docker
---

https://medium.com/@kelvin_sp/docker-introduction-what-you-need-to-know-to-start-creating-containers-8ffaf064930a

https://blog.usejournal.com/what-is-docker-in-simple-english-a24e8136b90b

When you are developing software, there comes a point when you want to ship the product. Some people say things like “it works on my machine” however this is not enough. The app needs to be able to work on all machines regardless of the platform or whatever.

So Docker is used to address the problem of “it works on my machine…”. How it does this is by containerisation.

Docker basically provides you with containers that are portable. So if you take this container from your machine to some other machine, it will work exactly how it worked on your machine. Docker also allows for social containers which means that you can share your docker containers with other people easily.


So to summarise, docker is a client side application. You install it on your machine and if you want to create a container, you can do so using a terminal command. Once you create a container, you can give this container to anyone else that has the docker client installed who can then take your container and run your program the exact way that it ran on your computer and the way you intended for it to be run.

This is helpful in production because you can install the docker client on your server and it will run the code EXACTLY how you ran it on your dev machine.

Real life example:

Imagine you have a class of students and you want to teach them how to use templates in django. You can make them each install django on their respective platforms and run into various problems OR you could make use of docker containers and create a docker container for the project yourself beforehand. Then all the students can just use this socially shared docker container to get up and running without having to worry about long installations etc.
