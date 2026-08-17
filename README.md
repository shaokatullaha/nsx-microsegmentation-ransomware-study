# Evaluating the Effectiveness of VMware NSX Micro-Segmentation for Ransomware Containment in Software-Defined Data Center

## Table of Contents

- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Research Question](#Research-Question)
- [Architecture](#Architecture)

## Overview

Ransomware remains one of the most disruptive threats to enterprise infrastructure, and Software Defined Data Centre (SDDC) environments are particularly exposed: interconnected virtual workloads create broad east-west network paths that allow ransomware to move laterally between systems once an initial foothold is gained.

This project evaluates whether **VMware NSX micro-segmentation**, enforced through the **Distributed Firewall (DFW)**, can meaningfully limit ransomware propagation in a virtualised enterprise environment. Rather than relying on perimeter defences alone, micro-segmentation applies fine-grained, workload-level security policy directly at the hypervisor — theoretically shrinking the "blast radius" available to an attacker who compromises a single VM.

The project builds a controlled VMware SDDC lab and tests four progressively stricter network security postures against a safe, benign lateral-movement simulation modelled on real ransomware behaviour (mapped to MITRE ATT&CK techniques). Containment effectiveness is measured empirically rather than assumed

## Problem Statement

Ransomware continues to cause major disruption to enterprise infrastructure, and Software Defined Data Centre (SDDC) environments are especially at risk: densely interconnected virtual workloads give attackers fast, largely unconstrained east-west paths to spread once a single VM is compromised. Traditional perimeter firewalls don't help here — they govern north-south traffic, not VM-to-VM. Prior work on SDN-based ransomware mitigation and on micro-segmentation more broadly rarely evaluates the mechanism actually deployed in real-world VMware SDDCs: the NSX Distributed Firewall. This project addresses that gap empirically.

## Research Question

**This project addresses the question:**

*To what extent does VMware NSX micro-segmentation reduce ransomware propagation blast radius and Mean Time to Contain (MTTC) in a Software-Defined Data Center (SDDC) environment when compared to a flat, unsegmented network architecture?*

## Architecture
