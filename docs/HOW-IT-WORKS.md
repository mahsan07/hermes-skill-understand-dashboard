# How Understand Dashboard Works

Launch an interactive dashboard that visualizes a codebase knowledge graph.

![Detailed systems blueprint for Understand Dashboard](../assets/system-blueprint.png)

## Stages

### 1. Load the existing graph artifact

**Primary surface:** `Code knowledge graph`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.
### 2. Start the local visualization service

**Primary surface:** `Graph service`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.
### 3. Render clusters nodes and relationships

**Primary surface:** `Filters and search`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.
### 4. Apply language path and component filters

**Primary surface:** `Interactive dashboard`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.
### 5. Inspect selected-node evidence

**Primary surface:** `Selected component detail`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.
### 6. Report dashboard URL and graph freshness

**Primary surface:** `Selected component detail`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.

## Failure handling

- **Authorization failure:** do not probe credentials or broaden access; report the missing authority.
- **Target ambiguity:** stop before mutation and request the minimum identifying information.
- **Tool or service failure:** retain error evidence, retry only safe transient failures, and cap retries.
- **Verification failure:** classify the run as incomplete even when the preceding operation returned success.

## Completion evidence

The handoff should contain the original request, inspection state, preview or plan, exact execution result, direct verification, and a final receipt naming limitations and withheld actions.
