# API Documentation

## Endpoints
### Matter Intake
- **Description**: Collect, validate and normalize emails from GRC; attach a runId and timestamp for traceability.
- **Type**: Processing

### Plan
- **Description**: Execute plan phase for the Plan-Execute pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Execute
- **Description**: Execute execute phase for the Plan-Execute pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Ingestion
- **Description**: Ingestion across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Entity Extraction
- **Description**: Entity Extraction across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Policy Check
- **Description**: Policy Check across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Risk Scoring
- **Description**: Risk Scoring across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Classification
- **Description**: Classification across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Privilege Log
- **Description**: Assemble final payload with status, artifacts, KPIs and audit trail; store to DMS; return response JSON for the client.
- **Type**: Processing
