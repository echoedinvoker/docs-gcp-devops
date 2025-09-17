# SLA

## Service Level Agreement

- Service level agreement

- It is contract with consequences of failing to meet the SLOs they contain

- SLO & SLA are quite similar

- But your SLAs should not be the same as your SLOs

## Key Differences

- **SLO is an internal objective**
  - If you can not meet SLO, team can slow down changes

- **SLAs violations are shared with your customers**
  - If you can not meet SLA, compensate need to be provided to customers

## Example
- https://cloud.google.com/terms/sla

## Important Principle
- **SLI should be higher than SLO & SLA**, means current indicator shows services are performing as expected

# SLA (Cntd...)

## SLI Performance Thresholds
- If SLI goes below SLO, slow own
- If SLI goes below SLA, notify customer & compensate

## SLA Setting Considerations
- Higher SLA Good but more likely you will violate it
- Lesser SLA means You will meet but customer will have less confident in your services

## Google Recommendation
- Google recommendation in case very high SLA
  - Down your service for some time
