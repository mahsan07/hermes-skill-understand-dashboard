# How Understand Dashboard Works

The visuals on this page are static SVGs, so they render directly on GitHub on phones and desktop browsers. Each one is generated from a model specific to this skill.

## System architecture

![Detailed system map for Understand Dashboard](../assets/system-map.svg)

### Components

- **1. Code knowledge graph:** participates in load the existing graph artifact.
- **2. Graph service:** participates in start the local visualization service.
- **3. Filters and search:** participates in render clusters nodes and relationships.
- **4. Interactive dashboard:** participates in apply language path and component filters.
- **5. Selected component detail:** participates in inspect selected-node evidence.

## Actor and data sequence

![Actor and data sequence for Understand Dashboard](../assets/operation-sequence.svg)

### 1. Load the existing graph artifact

**Primary surface:** `Code knowledge graph`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 2. Start the local visualization service

**Primary surface:** `Graph service`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 3. Render clusters nodes and relationships

**Primary surface:** `Filters and search`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 4. Apply language path and component filters

**Primary surface:** `Interactive dashboard`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 5. Inspect selected-node evidence

**Primary surface:** `Selected component detail`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 6. Report dashboard URL and graph freshness

**Primary surface:** `Code knowledge graph`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.

## Example output shape

![Illustrative output for Understand Dashboard](../assets/example-output.svg)

The example is a visual contract: a real run may look different, but it should expose comparable state, provenance, and verification information. It is not presented as evidence of a live external action.

## Decision and stop conditions

![Decision guide for Understand Dashboard](../assets/decision-guide.svg)

The workflow stops when the target is ambiguous, the relevant surface is unavailable or unauthorized, or the final artifact cannot be checked. A logged-in session or successful tool call is not by itself proof that the requested outcome is complete.

## Verification checklist

- Confirm every component shown in the system map exists in the target environment.
- Trace the actor sequence using actual tool output or artifact state.
- Compare the result with the example-output information contract.
- Re-read or reopen the final artifact instead of trusting an attempt message.
- Report omitted stages, unsupported capabilities, and remaining human decisions.
