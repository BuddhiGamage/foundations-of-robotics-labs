# Project 3: Kinematics for Manipulators

## Introduction

A manipulator is a mechanical system that is controlled by a set of joints. The joints are connected to each other by rigid links. The end-effector (EE) is the last link of the manipulator and it is the part of the manipulator that interacts with the environment. The kinematics of a manipulator is the study of the relationship between the joint angles and the position and orientation of the EE.

1. Introduction to the Kinova Gen3 lite manipulator - [intro gen3 lite notebook](01-intro-gen3lite.ipynb)
2. Direct kinematics - [direct kinematics notebook](02-direct-kinematics.ipynb)

## Installation

kinova ros package requires conan to build. To install conan, run the following commands:

```bash
# install conan
mamba install conan==1.59

# run conan config to set up for build kortex_ros package
conan config set general.revisions_enabled=1
conan profile new default --detect > /dev/null
conan profile update settings.compiler.libcxx=libstdc++11 default
```
