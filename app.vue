<script setup lang="ts">
import { ref } from 'vue'
interface DropdownOption {
  label: string
  value: string
}
const currencyOptions = ref<DropdownOption[]>([{ label: "Loading", value: "loading" }])
const selectedCurrency = ref<string>("loading")
</script>

<template>
  <FormKit
    type="dropdown"
    :value="selectedCurrency" 
    :options="currencyOptions"
  />
</template>