<template>
  <q-card class="q-pa-md shadow-2 my_card" bordered>
    <q-card-section class="text-center">
      <div class="text-grey-9 text-h5 text-weight-bold">Sign in</div>
      <div class="text-grey-8">Sign in below to access your account</div>
    </q-card-section>
    <q-card-section>
      <q-input dense outlined v-model="email" label="Email Address"></q-input>
      <q-input
        dense
        outlined
        class="q-mt-md"
        v-model="password"
        type="password"
        label="Password"
      ></q-input>
    </q-card-section>
    <q-card-section>
      <q-btn
        style="border-radius: 8px"
        color="dark"
        rounded
        size="md"
        label="Sign in"
        no-caps
        class="full-width"
      ></q-btn>
    </q-card-section>
    <q-card-section class="text-center q-pt-none">
      <div class="text-grey-8">
        Don't have an account yet?
        <a
          href="#"
          class="text-dark text-weight-bold"
          style="text-decoration: none"
          >Sign up.</a
        >
      </div>
    </q-card-section>
  </q-card>
</template>

<script lang="ts">
import { defineComponent } from "@vue/composition-api";

export default defineComponent({
  setup() {},
  name: "LoginModal",

  data() {
    return {
      email: null,
      password: null,
    };
  },
});
</script>
