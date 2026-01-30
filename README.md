# fetch-grocery-preparation-ai
Fetch-compatible robotics AI model for grocery preparation tasks in ManiSkill/MS-HAB simulations, supporting state-based observations and 13-dimensional normalized action control.
# Fetch Grocery Preparation AI Model

## Overview
This repository contains a Fetch mobile manipulator control model and task
definition for preparing groceries in ManiSkill / MS-HAB simulation environments.

The model follows the official AI Fetch Interface specification and supports
state-based observations with normalized 13-dimensional action outputs.

## Robot
- Fetch Mobile Manipulator

## Task
- Prepare groceries
- Sort grocery items by category
- Place items on counters, shelves, or storage areas

## Observation Mode
- state (flattened tensor or dictionary)

## Input
- Shape: (state_dim,) or (batch_size, state_dim)
- Data type: float32

## Output
- Shape: (13,)
- Range: [-1.0, 1.0]
- Control:
  - 7 arm joints
  - 1 gripper
  - 3 body joints
  - 2 base velocity controls

## Control Mode
- pd_joint_delta_pos

## Framework
- PyTorch

## Status
Submitted for AI Miner onboarding and Fetch robot evaluation.

## Author
GitHub: https://github.com/Aanika03
