<template>
<div>
  <SideNavMenu />
  <div class='header-background'>
    <h1 class='title'>Adhere.ly</h1>
  </div>
  <div class='main-view'>
    <SimpleReminderModal />
    <CardGridContainer />
  </div>
</div>
</template>

<script>
import SideNavMenu from '@/Components/SideNavMenu.vue'
import CardGridContainer from '@/Components/CardGridContainer.vue'
import SimpleReminderModal from '@/Components/Activities/SimpleReminderModal.vue'

export default {
  name: 'app',
  components: { SideNavMenu, CardGridContainer, SimpleReminderModal }
}

// npm compiled for production

</script>

<style lang='scss'>
@import url('https://fonts.googleapis.com/css?family=Pacifico&display=swap');
@import url('https://fonts.googleapis.com/css?family=Varela+Round&display=swap');

* {
 margin: 0;
 padding: 0;
 box-sizing: border-box;
 overflow-y: hidden;
 overflow-x: hidden;
 font-size: calc(12px + 1vw);
}

.header-background {
  text-align: center;
  width: 100%;
  height: 3.6rem;
}

.title {
  z-index: 1;
  font-size: 1.7rem;
  font-family: 'Pacifico';
  color: $darkgreen;
  line-height: 3.4rem;
}

.main-view {
  background-color: $lightgreen;
  height: 100vh;
  width: 100%;
}
</style>
