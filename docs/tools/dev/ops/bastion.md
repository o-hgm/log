# Bastion

Bastion is a tool to handle connections between an user and a set of resources.

It allows to split ssh connections in two:
* Ingress: User -> Bastion
* Egress: Bastion -> Instance

This allows to control who access which resource.

You can find more info about setup in [their github repository](https://github.com/ovh/the-bastion).