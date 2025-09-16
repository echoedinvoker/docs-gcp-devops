# Error budget

- One of goal of DevOps is implement gradual change

- Why outage occurs
  - Added new feature, change, new hardware, security patches

- More change leads to less stable system

- How to balance between change & stability

- We have to define metric for high system reliability.

- It is business Problem

- how much can the service fail before it begins to have a significant negative impact?

- How quickly do we need to be able to release new features?

- Depending on target, need to define error budget

# Error budget (Cntd...)

- Anytime your service is down, time require to recover it will be consumed from error budget

- After you define error budget
  - as long as you are within error budget, you are good to go for more changes
  - Once you run out of error budget, need to hold all future changes for deployment & make system stable first

- Larger error budget
  - means more downtime for service acceptable,
  - frequent changes possible.

- Less error budget,
  - means less downtime for service acceptable,
  - lesser changes allowed.

- Error budget make sure smaller & gradual changes deployed.
