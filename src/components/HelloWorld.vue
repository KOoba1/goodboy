<template>
  <v-container>
    <v-layout

      text-xs-center
      wrap
    >
    <div v-if="!quizStarted">
      <v-flex lg12 xs12 >
        <v-img
          :src="require('../assets/goodboy.gif')"
          class="my-3"
          contain
          height="200"
        ></v-img>
      </v-flex>

      <v-flex lg12 mb-4 xs12>

        <p class="subheading font-weight-regular">
          Who's the best boy?
          <br>Let's find out.

        </p>
      </v-flex>
       <v-btn @click="quizStarted = true">
              Start the quiz


        </v-btn>
    </div>
    <div v-if="quizStarted">
      <v-flex lg12 md12 xs12>
        <img src="../assets/Sam2.png"></img>
      </v-flex>
    </div>

    </v-layout>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      quizStarted:false,
      numberOfQuestions:10
    })
  }
</script>

<style>

</style>
