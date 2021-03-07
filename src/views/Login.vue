<template>
  <div>
    <h1>로그인</h1>
    <form @submit.prevent="submitForm">
      <div>
        <label for="username">username</label>
        <input type="text" v-model="username" id="username" />
      </div>
      <div>
        <label for="password">password</label>
        <input type="text" v-model="password" id="password" />
      </div>
      <button type="submit">로그인</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      username: "",
      password: ""
    };
  },
  methods: {
    submitForm() {
      console.log("로그인");
    }
  }
};
</script>

<style></style>
