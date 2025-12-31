---
name: 🏗️ Architecture Task
about: Propose a new feature, refactor, or any change that modifies source or tests
title: "[TASK] "
labels: enhancement, architecture
assignees: ""
---

## 📋 Summary

<!-- A clear, one-paragraph description of the proposed change. -->

## 🎯 Motivation

<!--
Why is this change needed?
- What problem does it solve?
- What use case does it enable?
- Link to any related issues or discussions.
-->

## 📐 Implementation Plan

<!--
Describe the technical approach in detail.
Be specific about which components are affected and how they interact.
-->

### Phase 1: <!-- e.g., "Parser Changes" -->

<!-- Describe the first phase of implementation -->

### Phase 2: <!-- e.g., "Compiler IR Updates" -->

<!-- Describe the second phase of implementation -->

### Phase 3: <!-- e.g., "Binding Updates" -->

<!-- Describe binding propagation if applicable -->

## 🎯 Target Vectors

<!--
List the specific files and directories that will be modified.
This helps reviewers and automated agents understand the scope.
-->

| File/Directory                | Change Type | Description                |
| :---------------------------- | :---------- | :------------------------- |
| `bindings/typescript/src/...` | Modify      | <!-- Brief description --> |
| `tests/spec/...`              | Add         | <!-- Brief description --> |
| `bindings/python/...`         | Modify      | <!-- Brief description --> |

## ✅ Acceptance Criteria

<!--
Define machine-checkable criteria where possible.
Include specific test commands and CI targets for automated verification.
-->

- [ ] **TypeScript Golden Master Updated:**
  ```bash
  cd bindings/typescript && npm run build:specs
  ```
- [ ] **Conformance Suite Passes:**
  ```bash
  ./strling test typescript
  ./strling test python
  ./strling test rust
  ```
- [ ] **No Regression in Existing Tests:**
  ```bash
  ./strling test all
  ```
- [ ] <!-- Additional criteria specific to this task -->

## 🔄 Migration & Compatibility

<!--
Describe any breaking changes and migration path.
If this is backwards-compatible, state that explicitly.
-->

- **Breaking Changes:** <!-- Yes/No, describe if yes -->
- **Deprecations:** <!-- List any deprecated APIs -->
- **Migration Guide:** <!-- Link or brief instructions -->

## 📚 Documentation Updates

<!--
List documentation that needs to be updated.
-->

- [ ] Update `spec/` grammar documentation
- [ ] Update binding-specific README files
- [ ] Update `manual` repository (if applicable)

## 🤖 Agent-Friendly Instructions

<!--
Optional: If this task should be completable by an AI coding agent,
include specific, step-by-step instructions here.
-->

```markdown
# Agent Instructions

1. Checkout the repository and run `./strling setup typescript`
2. Implement the changes in `bindings/typescript/src/...`
3. Run `npm run build:specs` to regenerate conformance tests
4. Verify with `./strling test typescript`
5. Propagate changes to Python binding
6. Verify with `./strling test python`
```

## 📎 Additional Context

<!--
Add any other context, mockups, or references here.
- RFC links
- Academic papers
- Similar implementations in other tools
-->
