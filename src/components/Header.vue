<template>
<div class="nav">
  <div class="notificationHeader">
  </div>
  <div class="logoWithNav">
    <div class="header">
    
      <h1>{{ msg }}</h1>    
    </div>
    <div class="buttonBar">
      <div class="navButtonContainer">
        <a href="" class="nav-link">Home</a>
      </div>
      <div class="navButtonContainer">
        <a href="" class="nav-link">Meet Us</a>
      </div>
      <div class="navButtonContainer">
        <a href="" class="nav-link">Services</a>
      </div>
      <div class="navButtonContainer">
        <a href="" class="nav-link">Contact Us</a>
      </div>
      <div class="navButtonContainer">
        <a href="" class="nav-link">COVID-19</a>
      </div>
    </div>
    <div class="callBtn">
      (+61) 411 483 530
    </div>
    <div class="bookAppointmentBtn">
      Make Appointment
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'Header',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.nav {
  width: 100vw;
  /* height: 10vh; */
  position: fixed;
  background-color: var(--firstColor);
  color:var(--secondColor);

}
.header {
  position: relative;
  display:block;
}
.buttonBar {
  position: relative;
  display:flex;
  flex-flow: row nowrap;
  justify-content: center;
  align-items: center;
}
.navButtonContainer {
  padding: 5px;
}

.nav-link{
  color:var(--navActive);
  text-decoration: none;
}

.logoWithNav {
  display: flex;
  flex-wrap: nowrap;
  flex-flow: row nowrap;
  justify-content: flex-start;
  align-items: center;
}

.callBtn {
  display: inline-block;
  font-weight: 600;
}

.bookAppointmentBtn {
  display: inline-block;
  font-weight: 600;
  text-align: center;
  vertical-align: middle;
  background-color: var(--secondColor);
  color:var(--firstColor);
  padding: 5px;
  border-radius: .25rem;
}
</style>
