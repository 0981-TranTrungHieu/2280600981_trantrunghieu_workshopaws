---
title: "Check monitoring and alerts"
date: 2026-07-14
weight: 4
chapter: false
pre: " <b> 5.5.4. </b> "
---

#### CloudWatch alarms

Check these alarms:

* EC2 CPU high
* EC2 memory high
* EC2 disk high
* EC2 status check failed
* RDS CPU high
* RDS connections high
* RDS free storage low
* RDS freeable memory low
* Lambda errors for `netflop-mediaconvert-notifier`
* Lambda errors for `netflop-subtitle-converter`

SNS topic:

```text
netflop-alerts
```

#### Checking steps

1. Open CloudWatch console.
2. Check alarm states.
3. Open Lambda logs.
4. Check SNS topic `netflop-alerts`.
5. Check Billing Dashboard/AWS Budgets.

![CloudWatch alarm 1](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.5-Deploy-test/5.5.4-monitoring-alerts/cw1.png)
![CloudWatch alarm 2](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.5-Deploy-test/5.5.4-monitoring-alerts/cw2.png)
![SNS](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.5-Deploy-test/5.5.4-monitoring-alerts/sns.png)
![Console](/2280600981_trantrunghieu_workshopaws/images/5-Workshop/5.5-Deploy-test/5.5.4-monitoring-alerts/console.png)

