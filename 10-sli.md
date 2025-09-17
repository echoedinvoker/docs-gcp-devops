# SLI

- Service level indicator

- Indicator internal to team

- SLI needs to be compared against SLO

- SLI are metrics which track over time (generally 5 minutes interval)

- SLI ranges from 0 to 100%

$$SLI = \frac{Total\ Good\ Event}{Total\ Valid\ Event} \times 100$$

- Let's say SLO – 96%
    - 96% of request should be serve within 300 ms latency.

- If Current SLI is 95% or anything less than 96%, system is under performing.

- SLI help us to find which service are not performing as per SLO

# SLI (Cntd...)

- Good SLI leads customer happy

- If Changes to SLI does not impact customer, SLI definition is not worth

- Different signal to track
    - Latency
    - Traffic
    - Errors
    - Saturation
    - Availability of system

- Selecting right SLO & SLI will lead to success
