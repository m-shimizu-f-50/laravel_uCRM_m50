<script setup>
import GestLayout from "@/Layouts/GuestLayout.vue"
import Label from "@/Components/InputLabel.vue"
import Input from "@/Components/TextInput.vue"

const emitTest = e => {
  console.log(e)
}

</script>


<template>
  <GestLayout>
    <Label value="件名">タイトル</Label>
    <Input @update:modelValue="emitTest" modelValue="初期値"></Input>
  </GestLayout>
</template>