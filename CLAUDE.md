# exo-work-onboarding-template

This is an onboarding template repository. It is **not** a Salesforce project.

## Available Tools

- **ClickUp**: Use the `code-mode-clickup` MCP tool (`execute_code`) to create tasks, search lists, and manage work items.
  - **Default list ID**: `901613782525`
  - **Required custom field**: Every task in this list requires "Team T-Shirt Estimate" (`id: 8e3d8f37-91fa-4df4-ba11-cfd72729cfc3`). Values: XS=0, S=1, M=2, L=3. Default to S (1) unless the user specifies otherwise.
    ```typescript
    custom_fields: [{ id: '8e3d8f37-91fa-4df4-ba11-cfd72729cfc3', value: 1 }]
    ```
  - **Key member IDs** (for assignees): Aniket Hendre=94997678, Karthik=94949390, Aakash=94927404, Priyanshu Gaur=95008808, Nikhil Mannikar=95051176, Vinay Mimani=94991964
- **ExoWork**: Use the `code-mode-exo-work` MCP tool for step completion and conversation management.
