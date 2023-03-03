<script setup lang="ts">
import { ref } from 'vue';

const account = ref('');
const password = ref('');

const handleSubmit = () => {};
</script>

<template>
  <div class="max__content">
    <div class="card">
      <h3 class="card__title">Log in</h3>
      <div class="card__content">
        <form class="form" @submit.prevent="handleSubmit">
          <div class="form__group">
            <label class="form__group">Account:</label>
            <input type="text" class="form__input" v-model="account" />
          </div>
          <div class="form__group">
            <label class="form__group">Password:</label>
            <input type="password" class="form__input" v-model="password" />
          </div>
          <div class="form__buttons">
            <button class="button button__blue">Log in</button>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
