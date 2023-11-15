<template>
  {{ dataChanged() }}
    <section class="home" id="home">
        <div class="container">
          <h1>Make Memories</h1>
          <p>Discover the place where you have fun & enjoy a lot</p>
    
          <div class="content grid">
            <div class="box">
              <span>ROOM TYPE </span> <br>
              <input v-model="source" list="newssources-list" v-on:input="sourceChanged" 
              name="source-selection" placeholder="Please specify news source ..."/>
              <datalist id="newssources-list">
                <option v-for="source in sources" v-bind:value="source.rtRoomType" v-bind:key="source.rtRoomTypeID"></option>
              </datalist>
            </div>
            <div class="box">
              <span>ARRIVAL DATE </span> <br>
              <input type="date" placeholder="29/20/2021">
            </div>
            <div class="box">
              <span>DEPARTURE DATE </span> <br>
              <input type="date" placeholder="29/20/2021">
            </div>
            <div class="box">
              <span>ADULTS</span> <br>
              <input type="number" placeholder="01">
            </div>
            <div class="box">
              <span>CHILDREN </span> <br>
              <input type="number" placeholder="0">
            </div>
            <div class="box">
              <button class="flex1">
                <span>Check Availability</span>
                <i class="fas fa-arrow-circle-right"></i>
              </button>
            </div>
          </div>
        </div>
      </section>
    
</template>

<script>
let once = false;

export default {
    //name : "Step1_menu",newssources-list
    name : "newssources-list",
    data () {
          return {
            sources: [],
            source: '',
            deepSource: ''
          }
        },
    methods: {
      dataChanged() {
        if (once == true) {
          return;
        }
        once = true;
        this.$axios.get("http://localhost:5000/api/roomtypes").then((response) => {           
            for (var i=0; i<response.data.length; i++){
              this.sources.push(response.data[i]);
            }
            console.log(this.sources);
           
        });
      },          
    },
  }

</script>




