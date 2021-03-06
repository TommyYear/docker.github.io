---
title: About Docker EE
description: Information about Docker Enterprise Edition Platform 2.0
keywords: enterprise, enterprise edition, ee, docker ee, docker enterprise edition, lts, commercial, cs engine
redirect_from:
  - /enterprise/supported-platforms/
green-check: '![yes](/install/images/green-check.svg){: style="height: 14px; margin:auto;"}'
install-prefix-ee: '/install/linux/docker-ee'
---

Docker Enterprise Edition (*Docker EE*) is designed for enterprise
development and IT teams who build, ship, and run business-critical
applications in production and at scale. Docker EE is integrated, certified,
and supported to provide enterprises with the most secure container platform
in the industry. For more info about Docker EE, including purchasing
options, see [Docker Enterprise Edition](https://www.docker.com/enterprise-edition/).

<!-- This is populated by logic in js/archive.js -->
<p id="ee-version-div"></p>

## Docker EE tiers

{% include docker_ce_ee.md %}

## Supported platforms

The following table shows all of the platforms that are available for Docker EE.
Each link in the first column takes you to the installation
instructions for the corresponding platform. Docker EE is an integrated,
supported, and certified container platform for the listed cloud providers and
operating systems.


### On-premises

These are the operating systems where you can install Docker EE.

| Platform                                                             |     x86_64 / amd64     |  IBM Power (ppc64le)   |     IBM Z (s390x)      |
|:---------------------------------------------------------------------|:----------------------:|:----------------------:|:----------------------:|
| [CentOS]({{ page.install-prefix-ee }}/centos.md)                     | {{ page.green-check }} |                        |                        |
| [Oracle Linux]({{ page.install-prefix-ee }}/oracle.md)               | {{ page.green-check }} |                        |                        |
| [Red Hat Enterprise Linux]({{ page.install-prefix-ee }}/rhel.md)     | {{ page.green-check }} | {{ page.green-check }} | {{ page.green-check }} |
| [SUSE Linux Enterprise Server]({{ page.install-prefix-ee }}/suse.md) | {{ page.green-check }} | {{ page.green-check }} | {{ page.green-check }} |
| [Ubuntu]({{ page.install-prefix-ee }}/ubuntu.md)                     | {{ page.green-check }} | {{ page.green-check }} | {{ page.green-check }} |
| [Microsoft Windows Server 2016](/install/windows/docker-ee.md)       | {{ page.green-check }} |                        |                        |

> Limitations on IBM Power architecture
>
> Neither UCP managers nor workers are supported on IBM Power.

### Docker Certified Infrastructure

Docker Certified Infrastructure is Docker’s prescriptive approach to deploying
Docker Enterprise Edition (EE) on a range of infrastructure choices. Each Docker
Certified Infrastructure includes a reference architecture, automation templates,
and third-party ecosystem solution briefs.

| Platform                                                                                | Docker Enterprise Edition |
|:----------------------------------------------------------------------------------------|:-------------------------:|
| [VMware](https://success.docker.com/article/certified-infrastructures-vmware-vsphere)   |  {{ page.green-check }}   |
| [Amazon Web Services](https://success.docker.com/article/certified-infrastructures-aws) |  {{ page.green-check }}   |
| [Microsoft Azure](https://success.docker.com/article/certified-infrastructures-azure)   |  {{ page.green-check }}   |
| IBM Cloud                                                                               |        Coming soon        |


## Docker Enterprise Edition release cycles

Docker EE is released quarterly. Releases use a time-based versioning
scheme, so for example, Docker EE version 17.03 was released
in March 2017. For schedule details, see
[Time-based release schedule](/engine/installation/#time-based-release-schedule).

Each Docker EE release is supported and maintained for one year and
receives security and critical bug fixes during this period.

The Docker API version is independent of the Docker platform version. The API
version doesn't change from Docker 1.13.1 to Docker 17.03. We maintain
careful API backward compatibility and deprecate APIs and features slowly and
conservatively. We remove features after deprecating them for a period of
three stable releases. Docker 1.13 introduced improved interoperability
between clients and servers using different API versions, including dynamic
feature negotiation.

## Upgrades and support

If you're a Docker DDC or CS Engine customer, you don't need to upgrade to
Docker EE to continue to get support. We will continue to support customers
with valid subscriptions whether the subscription covers Docker EE or
Commercially Supported Docker. You can choose to stay with your current
deployed version, or you can upgrade to the latest Docker EE version. For
more info, see [Scope of Coverage and Maintenance
Lifecycle](https://success.docker.com/Policies/Scope_of_Support).

## Where to go next

- [Install Docker](/engine/installation/index.md)
- [Get Started with Docker](/get-started/index.md)
