# `Project Objective` 

```
Develop, configure and protect a cloud environment with multiple subnets for
hosting corporate business assets.
```

# `{Required Tools}` 

```
Amazon Web Services (AWS)
Stable Internet Connection
```

```
---
```

# `Technical Implementation Summary:` 

```
An AWS virtual network (VPC) was designed and structured to be isolated with a
Classless Inter-Domain Routing (CIDR) block. Public-facing resources were
separated from private, back-end databases using nested subnets. Nested subnets
were used to isolate public-facing resources from private, back-end databases.
For traffic flow an Internet Gateway was set up and linked to custom Route
Tables, which allowed public subnets to communicate with the web, and private
subnets were kept hidden. Layered Network Access Control Lists (NACLs) and
stateful Security Groups were used to setup the traffic restrictions.
```

```
---
```

# `{Operational Relevance}` 

```
Network Segmentation & Attack Surface Reduction:
```

```
I segmented a large CIDR block into smaller public and private subnets to reduce
attack surface. This network model ensures that public web-based assets are not
connected to the corporate backend database.
```

# `Enterprise Routing & Access Control Design:` 

```
I configured the routing paths on the gateways and bounded them to the
appropriate route tables, which determine the exact way in which data can flow
in and out of the network. This highlights my growing understanding with
handling tedious traffic in corporate/busy networks.
```

# `Defense-in-Depth Implementation:` 

```
I created multi-layered cloud security approach through writing stateless subnet
filters with stateful host firewalls. I demonstrate that I'm was able to secure
critical workloads on the network by blocking all ports except the most secure
ones that are required for operation, such as HTTP and SSH.
```

