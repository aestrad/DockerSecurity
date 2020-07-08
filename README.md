# Container Threat Model

The purpose of threat modeling is to provide defenders with a systematic analysis of what controls or defenses need to be included, given the nature of the system, the probable attacker's profile, the most likely attack vectors, and the assets most desired by an attacker.

When we talk about containers we must consider the actors might be involved, 

* External actors attempting to access your deployment from outside.
* Internal actors who have access to some parts of the deployment.
* Malicious internal actors not limited to developers and administrators who have some leve of privilege to access the deployment.
* Application processes, daemons, account services that, might have programmatic access to the system

Each actor has a set of permissions that need to be review:

* What access do they have through credentials? For example, do they have access
to user accounts on the host machines your deployment is running on?
* What permissions do they have on the system? In Kubernetes, this could refer to
the role-based access control settings for each user, as well as anonymous users.
* What network access do they have? For example, which parts of the system are
included within a Virtual Private Cloud (VPC)?



## References

* Container Security Fundamental Technology Concepts that
Protect Containerized Applications by Lize Rice

* https://en.wikipedia.org/wiki/Threat_model
