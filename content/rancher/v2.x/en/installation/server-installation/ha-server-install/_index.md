---
title: HA Server Install
weight: 275
---
# High Availability Rancher Server Install

You have the option of installing Rancher Server in a High-Availability (HA) configuration. This configuration sets up multiple Rancher Servers, which ensure that you can always access Rancher, even when one of your Rancher Servers is down for maintentance.

Install Rancher in an HA configuration using the Rancher Kubernetes Engine (RKE). RKE is Rancher's own fast and light-weight Kubernetes installer. Use RKE to set up a new cluster that deploys Rancher as an addon.

Complete one of the following procedures to install Rancher in an HA configuration:

- [SSL Passthrough]({{< baseurl >}}/rancher/v2.x/en/installation/server-installation/ha-server-install/ssl-passthrough/)

	In this scenario, your High-Availability Rancher Servers handle SSL decryption rather than a Load Balancer.

- [SSL Termination]({{< baseurl >}}/rancher/v2.x/en/installation/server-installation/ha-server-install/ssl-termination/)

	In this scenario, your Load Balancer handles all SSL encryption, and then forwards on the communication within your Kubernetes cluster unencrypted.