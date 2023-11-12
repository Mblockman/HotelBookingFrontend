<template>
    <section class="home" id="home">
        <div class="container">
          <h1>Make Memories</h1>
          <p>Discover the place where you have fun & enjoy a lot</p>
    
          <div class="content grid">
            <div class="box">
              <span>ROOM TYPE </span> <br>
              <input type="string" placeholder="29/20/2021">
            </div>
            <div class="box">
              <span>STAY PERRIOD </span> <br>
              <input type="date" placeholder="29/20/2021">
            </div>
            <div class="box">
              <span>ADULTS</span> <br>
              <input type="number" placeholder="01">
            </div>
            <div class="box">
              <span>CHILDREN </span> <br>
              <input type="number" placeholder="01">
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
export default {
    name : "Step1_menu"
}
</script>




