# Day 9 - SIEM & Anomaly Detection Ruleset

> Day 9 of 14 in the **Zero to Production Infrastructure & Security** series.

Custom detection rules detecting privilege escalation and suspicious process spawning.

| | |
|---|---|
| **Day** | 9 of 14 |
| **Status** | Under construction |
| **Verification** | `python scripts/validate_rules.py` |
| **Tags** | `siem`  `wazuh`  `sysmon`  `detection-engineering`  `security` |

## Focus

- Threat hunting hypotheses
- Wazuh rule and Sysmon configuration authoring
- Security log field analysis
- Alert tuning and false positive reduction

## Status

Implementation lands during the Day 9 build session. Until then this
repository holds the agreed structure only - there is no placeholder code here
pretending to work.

The nightly pipeline appends the real verification result to [STATUS.md](STATUS.md).

## Layout

```
09-siem-detection-rules/
  README.md        this file
  LICENSE          MIT
  STATUS.md        machine-written verification record
  .gitignore       shared from the series root
  .gitattributes   forces LF endings so bash scripts run on Windows
```

## Verify

```bash
python scripts/validate_rules.py
```

The nightly job at 22:00 runs this command, records the result and
exit code in STATUS.md, then tags and pushes the repository.

## Licence

MIT. See [LICENSE](LICENSE).