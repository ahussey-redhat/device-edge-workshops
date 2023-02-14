# Workshop Exercise 1.1 - Preflight Checks

## Table of Contents

* [Objective](#objective)
* [Guide](#guide)
   * [Your Lab Environment](#your-lab-environment)
   * [Step 1 - Edge Device vs Virtual Device](#step-1---edge-device-vs-virtual-device)
   * [Step 2 - Investigating the Edge Device](#step-2---investigating-the-edge-device)
   * [Step 3 - Accessing the Virtual Device Host](#step-3---accessing-the-virtual-device-host)

## Objective

* Understand the lab topology, provided hardware (if applicable), and how to access virtual instances (again, if applicable).
* Understand how to use the workshop exercises.

These first few lab exercises will be exploring the lab and gathering baseline information for use in later excercises.

## Guide

### Your Lab Environment

In this lab, you work in a pre-configured lab environment and will have access to the following services:

| Service | Purpose |
| --- | --- |
| Ansible Controller | Automation controller for running Ansible automation |
| Gitea Source Control | SCM with a webUI for code storage |
| rpm-ostree Repo | Repo with various versions of an edge image available over an http server |

Since this is a shortened lab, the Image Builder related steps have already been completed, and images are hosted and ready for consumption.

> **Note**
>
> If you need more information on new Ansible Automation Platform components, bookmark this landing page [https://red.ht/AAP-20](https://red.ht/AAP-20)

### Step 1 - Edge Device vs Virtual Device

- If physical devices are available at your lab station, proceed to [Step 2 - Investigating the Edge Device](#step-2---using-the-terminal)
- If a physical device is not available at your lab station, proceed to [Step 3 - Accessing the Virtual Device Host](#step-3---accessing-the-virtual-device-host)

### Step 2 - Investigating the Edge Device

- A device should be available at your station, along with the usual suite of peripherals (IE; keyboard, mouse, monitor and cables).
- There may be doubling up of students to devices depending on availability.

### Step 3 - Accessing the Virtual Device Host

A bare metal instance has been created in RHPDS that will host virtual instances meant to represent an edge device. Your "Workbench Information" page that lists credentials to the various services includes a link to the Image Builder Cockpit interface. This is the machine on which your VMs are hosted. You can, alternatively, SSH to the instance using the Edge Manager SSH Access and interact with your VMs using traditional command line tooling, virt-manager with a remote connection configured on your host, or any other access method you might prefer.

It is highly encouraged that the Cockpit web interface be used to complete the workshop exercises. Cockpit provides:
- An easy to access interface to managing virtual machines running on RHEL
- Tooling for creating, starting, and stopping virtual machines
- A web based console for bootstraping and troubleshooting

For more information on Cockpit, check out [Intro to Cockpit](https://www.redhat.com/sysadmin/intro-cockpit)

---
**Navigation**

[Next Exercise](../1.2-controller-intro)

[Click here to return to the Workshop Homepage](../README.md)
