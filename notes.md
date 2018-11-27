# Introduction to Cloud Computing with OpenStack and Juju @ GARR
## What is OpenStack?
`OpenStack is a cloud operating system that controls large pools of compute, storage, and networking resources throughout a datacenter, all managed through a dashboard that gives administrators control while empowering their users to provision resources through a web interface.
`
## GARR Cloud Infrastructure
- Declarative Modelling: describes the **what** and not the **how**
to do in order to build and deploy a cloud infrastructure. This entails several benefits:
  - **Cross platform** deployment (Portability)
  - Changes are **propagated** by means of constraints (Consistency)
  - The mapping between the model to the actual physical infrastructure is offloaded to the **orchestrator** (Automation)
  - Up/Downscaling (Evolution)

  ### Automation Tools
  - Puppet (Software, Config, State)
  - Chef (Software, Config, State)
  - Ansible (Software, Config, State)
  - **Juju** (Software, Config, State & Orchestration)

    #### Procedural vs Declarative Modelling
    **Ansible**
    1. Connect to each server
    2. Install packages  for a WebApp
    3. Configure WebApps, styles (`sed`)
    4. Create DB credentials
    5. Connect DB to server
    6. Create table and populate data

    **Juju**
    1. Specify:
      - Applications
      - Number of Servers
    2. (Optional) Set Parameters
    3. -

  ### Kubernetes
  - Container **orchestrator**
  - Manages **applications**, not **machines**

  The GARR container platform is based on **Kubernetes** and deployed on bare metal.