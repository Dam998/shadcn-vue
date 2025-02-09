---
title: Switch
description: A control that allows the user to toggle between checked and not checked.
source: apps/www/src/lib/registry/default/ui/switch
primitive: https://www.radix-vue.com/components/switch.html
---

<ComponentPreview name="SwitchDemo" />

## Installation

<TabPreview name="CLI">
<template #CLI>

```bash
npx shadcn-vue@latest add switch
```
</template>

<template #Manual>

<Steps>

### Install the following dependency:

```bash
npm install radix-vue
```

### Copy and paste the following code into your project

 <<< @/lib/registry/default/ui/switch/Switch.vue

</Steps>

</template>
</TabPreview>

## Usage

```vue
<script setup lang="ts">
import { Switch } from '@/components/ui/switch'
</script>

<template>
  <Switch />
</template>
```

# Add icon inside switch thumb

```vue
<template>
  <Switch :checked="isDark" @update:checked="toggleTheme">
      <template #thumb>
          <Icon v-if="isDark" icon="lucide:moon" class="size-3"></Icon>
          <Icon v-else icon="lucide:sun" class="size-3"></Icon>
      </template>
  </Switch>
</template>
```

## Examples

### Form

<ComponentPreview name="SwitchForm" />
