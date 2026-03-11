---

# Sequential Workflow in LangGraph – Notes

## What is a Sequential Workflow?

A Sequential Workflow is a workflow in which **nodes execute one after another in a fixed order**.

Each node performs a task and then passes the updated state to the next node.

Flow example:

```
Node 1 → Node 2 → Node 3 → End
```

This means the second node runs **only after the first node finishes**, and the third node runs **after the second node finishes**.

---

# Characteristics of Sequential Workflow

* Tasks are executed **step-by-step**.
* The order of execution is **fixed and predefined**.
* Each node receives the **state from the previous node**.
* It is the **simplest workflow structure** in LangGraph.

---

# Components in Sequential Workflow

## 1. State

State stores the data shared between nodes during the workflow.

Example data:

* user input
* intermediate results
* processed information

---

## 2. Nodes

Nodes are the **individual processing steps**.

Each node:

* reads the state
* performs a task
* updates the state

---

## 3. Edges

Edges connect nodes and define the **sequence of execution**.

Example sequence:

```
Start → Node A → Node B → Node C → End
```

---

## 4. Entry Point

The entry point defines **where the workflow begins**.

Execution starts from this node.

---

# Advantages of Sequential Workflow

* Simple to design and understand
* Easy to debug
* Suitable for **step-by-step processing tasks**

---

# Example Use Cases

Sequential workflows can be used in:

* Text processing pipelines
* Data processing steps
* Multi-step reasoning tasks
* AI content generation pipelines

Example:

```
User Question → Analyze Question → Generate Answer → Format Output
```

---

# Summary

Sequential Workflow is a workflow where **nodes run in a fixed order one after another**.

Main components:

* State – stores data
* Nodes – perform tasks
* Edges – define order
* Entry Point – starting node

This type of workflow is useful for **simple and structured AI processes**.

---

If you want, I can also give you **very short “1-page revision notes for LangGraph (all topics)”** so your **GitHub notes + exam preparation become very efficient.**
