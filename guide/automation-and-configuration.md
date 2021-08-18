#### What it is

Automation and configuration tools speed up the creation and configuration of compute
resources (virtual machines, networks, firewall rules, load balancers, etc.). Tools in
this category either handle different parts of the provisioning process or try to control
everything end-to-end. Most provide the ability to integrate with other projects and
products in the space.

#### Problem it addresses

Traditionally, IT processes relied on lengthy and labor intensive manual release cycles,
typically between three to six months. Those cycles came with lots of human processes and
controls that slowed down changes to production environments. These slow release cycles
and static environments aren’t compatible with cloud native development. To deliver on
rapid development cycles, infrastructure must be provisioned dynamically and without
human intervention.

#### How it helps

Tools of this category allow engineers to build computing environments without human
intervention. By codifying the environment setup it becomes reproducible with the click
of a button. While manual setup is error prone, once codified, environment creation
matches the exact desired state -- a huge advantage.

While tools may take different approaches, they all aim at reducing the required work
to provision resources through automation.

#### Technical 101

As we move from old-style human-driven provisioning to a new on-demand scaling model
driven by the cloud, the patterns and tools we used before no longer meet our needs.
Most organizations can’t afford a large 24x7 staff to create, configure, and manage
servers. Automated tools like Terraform reduce the level of effort required to scale
tens of servers and networks with hundreds of firewall rules. Tools like Puppet, Chef,
and Ansible provision and/or configure these new servers and applications
programmatically as they are spun up and allow them to be consumed by developers.

Some tools interact directly with the infrastructure APIs provided by platforms like
AWS or vSphere, while others focus on configuring the individual machines to make them
part of a Kubernetes cluster. Many, like Chef and Terraform, can interoperate to provision
and configure the environment. Others, like OpenStack, exist to provide an
Infrastructure-as-a-Service (IaaS) environment that other tools could consume.
Fundamentally, you'll need one or more tools in this space as part of laying down the
computing environment, CPU, memory, storage, and networking, for your Kubernetes clusters.
You'll also need a subset of these to create and manage the Kubernetes clusters
themselves.

There are now over 5 CNCF projects in this space, more if you count projects like Cluster
API which don’t appear on the landscape. There is also a very robust set of other open
source and vendor provided tools.
