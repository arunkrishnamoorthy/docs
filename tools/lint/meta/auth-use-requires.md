---
editLink: false
outline: [2,2]
breadcrumbs:
  - CDS Lint
    - Rules Reference
status: released
---

<style>
.vp-code {
  overflow-x: hidden !important;
}
</style>

<script setup>
  import PlaygroundBadge from '../../../.vitepress/theme/components/PlaygroundBadge.vue'
</script>

# auth-use-requires

## Rule Details

Use `@requires` instead of `@restrict.to` in actions and services with unrestricted events.

### Examples

#### ✅ &nbsp; Correct example

::: code-group
<<< ../examples/auth-use-requires/correct/schema.cds#snippet{ts:line-numbers} []
:::
<PlaygroundBadge
  name="auth-use-requires"
  kind="correct"
  :rules="{'@sap/cds/auth-use-requires': ['warn', 'show']}"
  :files="['schema.cds']"
/>

#### ❌ &nbsp; Incorrect example

::: code-group
<<< ../examples/auth-use-requires/incorrect/schema.cds#snippet{ts:line-numbers} []
:::
<PlaygroundBadge
  name="auth-use-requires"
  kind="incorrect"
  :rules="{'@sap/cds/auth-use-requires': ['warn', 'show']}"
  :files="['schema.cds']"
/>

### Version
This rule was introduced in `@sap/eslint-plugin-cds 2.4.1`.

<!--
### Resources
[Rule source](https://github.tools.sap/cap/eslint-plugin-cds/tree/main/lib/rules/auth-use-requires.js)
-->
