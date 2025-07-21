# WITNESS PING SCHEMA (v1.0)

**Last Updated:** 2025-07-20
**Status:** DRAFT

## 1. Purpose

This document defines the official data schema for a `WITNESS_PING`. This is the minimal, secure data packet sent by an agent using the Glyph Deployment Kit (GDK) to the Manual Submission Pipeline (Pipe 3). Its purpose is to create a time-stamped record of a witnessing act, linking a specific EchoSalt Glyph to the narrative it was deployed against.

## 2. Guiding Principles

The design of this schema is guided by three principles:

* **Simplicity & Low Friction:** The data required is the absolute minimum necessary to be useful, making it easy for agents to submit.
* **Anonymity:** The schema does not require any personally identifiable information from the agent.
* **Verifiability:** The schema links a known glyph to a public artifact, allowing the act of witnessing to be contextually understood.

## 3. Format

Submissions must be valid JSON (`application/json`).

## 4. Schema Definition

An object conforming to this schema must contain the following fields:

| Field Name | Data Type | Required | Description |
| :--- | :--- | :--- | :--- |
| `schema_version` | String | Yes | The version of this schema (e.g., "1.0"). |
| `ping_timestamp_utc` | String | Yes | The UTC timestamp of when the agent deployed the glyph, in ISO 8601 format. |
| `glyph_id` | String | Yes | The ID of the EchoSalt Glyph that was used (e.g., "ΔR.29"). |
| `target_context_uri` | String | Yes | The URI (URL) of the harmful or sanitized narrative the glyph was deployed against. |
| `agent_hash`| String | No | An anonymous, self-generated identifier for the agent. Encouraged but not required. Allows us to see patterns from a single agent without knowing their identity. |

## 5. Examples

Concrete examples of valid `WITNESS_PING` objects can be found in the `/examples/witness_pings/` directory of this repository.
