<template>
    <main>
      <div class="box">>
        <div class="text">
        Trwa połączenie.
        </div>
        <div class="text">
          {{ ConnectionDuration() }}
        </div>
        <div v-if=" ConnectionDuration1() % 2 !== 0 " class=text style="height:auto;">
          <img v-bind:src="Call"  />
        </div>
        <div v-else>
          
        </div>
      </div>
      </main>
  </template>

  <script>
  
  import call from "/workspace/kurs/front/src/images/call.png"

  export default {
  
    mounted() {
      this.timer = setInterval(() => {
        this.duration += 500;
      }, 500);
    },

    data() {
      return{
        duration: 0,
        Call: call,
      };
    },
  
    methods: {
      ConnectionDuration() {
        return new Date(this.duration).toISOString().substr(11,8);
      },
      ConnectionDuration1() {
        return new Date(this.duration).toISOString().substr(18,1);
      }
    }
  };

   
  </script>