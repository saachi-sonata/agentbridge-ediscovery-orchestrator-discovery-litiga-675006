# Architecture Documentation

## Overview
This Plan-Execute implements eDiscovery Orchestrator • Discovery (Litigation) for Legal & Compliance use cases.

## Components
1. **Matter Intake**: Collect, validate and normalize emails from GRC; attach a runId and timestamp for traceability.
2. **Plan**: Execute plan phase for the Plan-Execute pattern: persist interim state, enforce guardrails, and emit structured JSON results.
3. **Execute**: Execute execute phase for the Plan-Execute pattern: persist interim state, enforce guardrails, and emit structured JSON results.
4. **Ingestion**: Ingestion across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
5. **Entity Extraction**: Entity Extraction across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
6. **Policy Check**: Policy Check across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
7. **Risk Scoring**: Risk Scoring across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
8. **Classification**: Classification across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
9. **Privilege Log**: Assemble final payload with status, artifacts, KPIs and audit trail; store to DMS; return response JSON for the client.

## Data Flow
- Input: Matter Intake
- Processing: 9 sequential steps
- Output: Privilege Log
