# JupyterHubPi

Jupyter Hub Lab inside Raspberry Pi

## Purpose is to have a quick solution to work together at any local site

With jupyter lab and a shared file system its quick to use in a collaborative meeting.  
Using a small SBC means no one hase to offer his/her laptop to host jupyterhub/lab.  

Runs locally, keeping it simple.  

## Pre-requisites

- Some familiarity with the command line.
- A server running Ubuntu 20.04+ where you have root access (Ubuntu 22.04 LTS recommended).
- At least 1GB of RAM on your server.
- Ability to ssh into the server & run commands from the prompt.
- An IP address where the server can be reached from the browsers of your target audience.

## Raspberry Specifics

Per se the hardware is quite limited, but should have enough performance..

32 bit ARMhf is not supported (we tried). Other from that it should be fine to run JuptierHub on it.

## Installing The Littlest JupyterHub

Using a script is the fastest Method of setting up the system. 

The following [Tutorial TLJH](https://tljh.jupyter.org/en/latest/install/custom-server.html) contains all necessary steps.

## Subsystems

JupyterHub is made up of four subsystems:

- a Hub (tornado process) that is the heart of JupyterHub
- a configurable http proxy (node-http-proxy) that receives the requests from the client’s browser
- multiple single-user Jupyter notebook servers (Python/IPython/tornado) that are monitored by Spawners
- an authentication class that manages how users can access the system
