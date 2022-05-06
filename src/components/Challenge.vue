<script>
export default {
  name: "ChallengeComponent",
  props: {
    msg: String,
  },

  data() {
    return {
      count: 0,
      result: 0,
    };
  },
  methods: {
    checkResult() {
      this.result = 2;
    },
  },
};
</script>
<template>
  <div class="challenge">
    <div class="question">
      <h2>{{ msg }}</h2>
      <p>Bora somar:</p>
      <code> 1 + 1 </code>
    </div>
    <div class="verification">
      <button @click="checkResult">Checar</button>
    </div>
    <div class="answer">
      <h4>Resultado</h4>
      <code>
        {{ result }}
      </code>
    </div>
  </div>
</template>
<style scoped>
.question {
    background: #ddd;
}
.verification {
    background: #ddd;
}
.answer {
    background: #ddd;
}
</style>