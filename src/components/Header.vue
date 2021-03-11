<template>
<div class="nav">
  <div class="notificationHeader">
  </div>
  <div class="logoWithNav">
    <div class="header">
    
      <h1>{{ msg }}</h1>    
    </div>
    <div class="buttonBar">
      <div class="navContainer">
        <a href="" class="nav-link-standard">Home</a>
      </div>
      <div class="navContainer">
        <a href="" class="nav-link-standard">Meet Us</a>
      </div>
      <div class="navContainer">
        <a href="" class="nav-link-standard">Services</a>
      </div>
      <div class="navContainer">
        <a href="" class="nav-link-standard">Contact Us</a>
      </div>
      <div class="navContainer">
        <a href="" class="nav-link-standard">COVID-19</a>
      </div>
    </div>
    <div class="navContainer">
      (+61) 411 483 530
    </div>
    <div class="navFocusContainer">
      <a href="" class="nav-link-focus" target="_blank"> Make Appointment </a>
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

.nav {
  width: 100vw;
  /* height: 10vh; */
  position: fixed;
  background-color: var(--firstColor);
  color:var(--secondColor);
  display: flex;
  align-items: center;
  justify-content: center;

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
.navContainer {
  padding: 5px;
}

.nav-link-standard{
  color:var(--navActive);
  text-decoration: none;
}

.nav-link-focus{
  color:var(--navActiveFocus);
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

.navFocusContainer {
  display: inline-block;
  font-weight: 600;
  text-align: center;
  vertical-align: middle;
  background-color: var(--secondColor);
  color:var(--firstColor);
  padding: 10px;
  border-radius: .25rem;
}

.navFocusContainer > a:hover {
  color: #fff;
}
.navContainer > a:hover {
  color: #fff;
}
</style>
