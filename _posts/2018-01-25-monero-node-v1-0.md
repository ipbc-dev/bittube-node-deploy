---
layout: post
title: Monero Node v1.0
---

First launch of the Cloudformation template and accompanying site hosted on Cloudfront. This template deploys Monero v0.11.1.0, "Helium Hydra". Features of the template include:

* Regional mapping for Amazon Linux AMI, supports us-east-1, us-east-2, us-west-1, us-west-2, ca-central-1, and eu-west-2
* Open node security group (daemon and rpc exposed publicly)
* Private access security group (SSH for management IP)
* 50 GB Elastic Block Store gp2 (SSD) disk
* Customizable instance type, SSH key, and networking
* User data shell script for running persistent Monero daemon
* Cloudwatch logs agent for logging daemon activity
* IAM instance profile for instance specific API requirements (Cloudwatch)
* Elastic IP for persistent IP assignment
