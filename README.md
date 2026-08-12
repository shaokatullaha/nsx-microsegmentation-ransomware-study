# Evaluating the Effectiveness of VMware NSX Micro-Segmentation for Ransomware Containment in Software-Defined Data Center

## Table of Contents

- [Overview](#overview)
- [Problem Statement](#problem-statement)
## Overview

Ransomware remains one of the most disruptive threats to enterprise infrastructure, and Software Defined Data Centre (SDDC) environments are particularly exposed: interconnected virtual workloads create broad east-west network paths that allow ransomware to move laterally between systems once an initial foothold is gained.

This project evaluates whether **VMware NSX micro-segmentation**, enforced through the **Distributed Firewall (DFW)**, can meaningfully limit ransomware propagation in a virtualised enterprise environment. Rather than relying on perimeter defences alone, micro-segmentation applies fine-grained, workload-level security policy directly at the hypervisor — theoretically shrinking the "blast radius" available to an attacker who compromises a single VM.

The project builds a controlled VMware SDDC lab and tests four progressively stricter network security postures against a safe, benign lateral-movement simulation modelled on real ransomware behaviour (mapped to MITRE ATT&CK techniques). Containment effectiveness is measured empirically rather than assumed

## Problem Statement
