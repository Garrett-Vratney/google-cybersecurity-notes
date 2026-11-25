# Chapter 6, Module 4 · Logs, IDS, and SIEM Queries

[Back to index](../README.md)

## Topics Covered

- Log sources and formats
- Host-based and network-based IDS
- Signature and anomaly detection
- Suricata alerts
- Splunk SPL and Google SecOps UDM

## Study Notes

Logs capture events and can be one source of telemetry. Useful fields include timestamp, actor, action, source, destination, and outcome. Host-based IDS sees local activity, while network-based IDS examines traffic. Signature detection matches defined patterns and anomaly detection flags departures from a baseline. Suricata rules have an action, header, and options, with enforcement depending on operating mode. In Splunk, `index=main fail | stats count by host` counts matching events by host. Google SecOps UDM provides normalized fields for cross-source searches.

## Key Takeaways

- Verify the time range and field meaning before interpreting search results.
- Tune anomaly thresholds against normal activity and validate signature alerts in context.
- Keep raw events available when normalization hides useful details.

## Source

Personal course notes in `Ch 6 Module 4.docx`.
