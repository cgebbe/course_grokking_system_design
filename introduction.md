# Introduction

> system design = process of defining components, APIs and data models to build large scale system

- targets
  - effective = meets requirements
  - maintainable = flexible to change (e.g. scale, add features)
  - reliable = little downtime = handles errors (which will always occur!)
- system building blocks (in this course 16)
  - load balancer
  - ...
- recommended prerequesite:
  - distributed systems
    - https://www.educative.io/courses/distributed-systems-practitioners
  - computer networking
  - operating systems

# Interview

- recommended steps
  - solidify requirements
  - scope problem (i.e. which features are left to focus on core)
  - let interviewer take part in thought process
- recommended strategy
  - 1. Ask refining questions
    - put on product manager hat and prioritize requirements
    - split requiremenst into
      - direct/functional ones (e.g. ability to send messages in real-time)
      - indirect/nonfunctional ones (e.g. messaging performance shouldn't degrade with high load)
  - 2. Understand data characteristics
    - size, read-write-speed, consistency, durability, regulatory requirements, ...
    - how will data be consumed by subsystems or end users?
  - 3. Discuss components
    - which to pick, where to place, how they interact
  - 4. Discuss trade-offs
    - each choice has pros and cons, discuss them and your pick.
    - e.g.: current system has low costs, but cannot scale 10x load
      - mitigate shortcoming via monitoring load and scale-up-plan

# Abstractions
