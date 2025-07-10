---
mode: 'agent'
description: 'Review Azure Architecture Center multitenant service-specific guidance to ensure it is up-to-date with multitenant features provided by the service and guidance is still relevant.'
tools: ['codebase', 'fetch', 'githubRepo', 'search', 'searchResults', 'microsoft.docs.mcp', 'azure_get_code_gen_best_practices', 'azure_get_deployment_best_practices', 'azure_query_learn']
---

# Review Azure Architecture Center Multitenant Service-Specific Guidance document

Analyze Azure Architecture Center multitenant service guidance in ${file} for currency and relevance. Produce a table of Azure service updates since last review that uniquely benefit multitenant solutions. **DO NOT modify the document.**

## Context

Azure Architecture Center provides multitenant best practices at `https://learn.microsoft.com/en-us/azure/architecture/guide/multitenant/overview`. Access via `microsoft.docs.mcp` tool.

**Focus Area**: Service-specific guidance section only.

**Important**: "Tenant" = your customers/user groups (not Microsoft Entra tenants).

## Review Process

1. **Extract review date** from document front matter (`ms.date:` field, format: mm/dd/yyyy)
2. **Identify Azure service** from document title
3. **Search for updates** using `microsoft.docs.mcp`:
   - Find service "What's New" pages
   - Locate multitenant-specific guidance
   - Check for feature updates since review date
4. **Continue searching** until all sources exhausted

## Relevance Criteria

Include changes that add features uniquely useful for multitenant solutions. Exclude:
- General improvements not specific to multitenancy
- Already documented features
- Non-multitenant benefits

## Output Format

**If changes found:**

| Status | Change Type | Reason why it matters | Date Added | Reference Doc |
|--------|-------------|----------------------|------------|---------------|
| ✅ | Feature | Key Vault supports tagging secrets, with custom metadata, so you can use a tag to track the tenant ID for each tenant-specific secret. However, Key Vault doesn't support querying by tags, so this feature is best suited for management purposes, rather than for use within your application logic. | 2025-05-23 | [Azure Key Vault throttling guidance](https://learn.microsoft.com/en-us/azure/key-vault/secrets/about-secrets#secret-tags) |

**Status Icons:**
- ✅ Already documented - no change needed
- ➡️ Already documented - change needed
- ❌ Not documented - should be added
- ❓ Documentation status unclear
- ⛔ Feature Not applicable

**If no relevant changes:** 🎇 No changes needed.

**Post-table:** Offer to provide change text if updates required.
