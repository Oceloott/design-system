<template>
  <div class="flex flex-column card">
    <FormText tag="h1" text="Sign in" color="secondary-black" top="0" bottom="0"/>
    <div class="flex flex-row flex-center">
      <FormText tag="p" text="Not signed up ?" color="secondary-black" bottom="3" top="3"/>
      <NuxtLink to="/Sign_up" class="underline text-color--secondary-black margin-left--1">Register</NuxtLink>
    </div>
    <form class="flex flex-column">
      <FormText tag="p" text="Email" color="secondary-black" classes="bold" bottom="2" top="0"/>
      <input type="email" name="email" placeholder="johndoe@mail.com">
      <FormText tag="p" text="Password" color="secondary-black" classes="bold" top="3" bottom="2"/>
      <input type="password" name="email" placeholder="**********">
      <FormText tag="span" text="Forget password ?" color="secondary-black" classes="underline" top="1"/>
      <FormButton text="Sign in" type="button" look="primary" size="medium" disabled="disabled" />
    </form>
  </div>
</template>

<script>
  import FormButton from '@/components/FormButton.vue'
  import FormText from '@/components/FormText.vue'
  import FormInput from '@/components/FormInput.vue'

  export default {
    name: 'input',
    components: {
      FormButton,
      FormText,
      FormInput
    },
  }

</script>
