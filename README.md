# argo-sync

This repository contains everything relevant for ArgoCD.

## Dev and testing

Due to how ArgoCD works, inactive apps need to be commented out within the app of apps. Furthermore, to allow for testing, a dev directory was setup, together with all required configurations. As such, the workflow for testing is as follows:

- Work on branch called "testing"
- Work in directory "apps/dev"
- Once done:
    - Move to own directory in apps
    - PR to main

## GitFlow

From top to bottom:

| Branch         | Merge into |
|----------------|------------|
| feature branch | dev        |
| dev            | main       |
