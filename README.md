# [IROS23] Meta Depth Completion - ResLAN
__Wolfgang Boettcher, Lukas Hoyer, Ozan Unal, Dengxin Dai__

*IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS2023)*

## News

- June 2023: Our paper was accepted to IROS2023

## Introduction

Depth estimation is one of the essential tasks to
be addressed when creating mobile autonomous systems. While
monocular depth estimation methods have improved in recent
times, depth completion provides more accurate and reliable
depth maps by additionally using sparse depth information
from other sensors such as LiDAR. However, current methods
are specifically trained for a single LiDAR sensor. As the
scanning pattern differs between sensors, every new sensor
would require re-training a specialized depth completion model,
which is computationally inefficient and not flexible. 

In this paper,
we propose to dynamically adapt the depth completion model to
the used sensor type enabling LiDAR adaptive depth completion.
Specifically, we propose a meta depth completion network
that uses data patterns derived from the data to learn a
task network to alter weights of the main depth completion
network to solve a given depth completion task effectively. The
method demonstrates a strong capability to work on multiple
LiDAR scanning patterns and can also generalize to scanning
patterns that are unseen during training. While using a single
model, our method yields significantly better results than a
non-adaptive baseline trained on different LiDAR patterns. It
outperforms LiDAR-specific expert models for very sparse cases.
These advantages allow flexible deployment of a single depth
completion model on different sensors, which could also prove
valuable to process the input of nascent LiDAR technology with
adaptive instead of fixed scanning patterns.
