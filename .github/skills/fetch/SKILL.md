---
name: fetch
description: "Fetch Jira tickets using Atlassian MCP tools. Use when: retrieving Jira issues, querying tickets by JQL, looking up issue details, pulling ticket data for analysis or implementation."
argument-hint: "Jira issue key (e.g. OC-74) or JQL query"
---

# Fetch

Retrieve Jira ticket details using the Atlassian MCP tools and return structured data for downstream agents.

## When to Use

- User provides a Jira issue key (e.g. `PROJ-123`)
- User wants to search issues by JQL
- User needs ticket details before starting analysis or implementation
- Starting any FlowPilot pipeline run

## Procedure

1. Resolve the Atlassian cloud ID using `mcp_atlassian-mcp_getAccessibleAtlassianResources`
2. Fetch the ticket using `mcp_atlassian-mcp_getJiraIssue` or search with `mcp_atlassian-mcp_searchJiraIssuesUsingJql`
3. Extract key, summary, status, priority, assignee, issue type, description, labels, and timestamps
4. Return structured data for downstream consumption

Full agent instructions: [fetch.md](../../../fetch/fetch.md)
