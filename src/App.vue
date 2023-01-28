<template>
  <div class="select-character">
    <CharacterItem
      :status="'default'"
      :level="75"
      :number="1"
      :hoursInGame="666"
      :cash="500000"
      :moneyInBank="1"
      :organization="'LSPD'"
      :characterName="'Demon'"
    />
    <CharacterItem
      :status="'deleting'"
      :level="75"
      :number="1"
      :hoursInGame="666"
      :cash="500000"
      :moneyInBank="1"
      :organization="LSPD"
      :characterName="'Demon'"

      :deletedTime="'6/12 23:54'"
    />
    
  </div>
  
</template>

<script>
import CharacterItem from './components/CharacterItem.vue';

export default {
  name: 'App',
  components: {
    CharacterItem
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600;700;800;900&display=swap');

body {
  outline: none;
  margin: 0;
  padding: 0;
}

#app {
  font-family: 'Montserrat', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 100%;
  height: 100vh;
  background: url("@/assets/background.png");
  background-color: #0B0C0D;
  background-position: right center;
  background-size: cover;
  background-repeat: no-repeat;
  display: flex;
  justify-content: center;
}

.select-character {
  width: 91%;
  display: flex;
  align-items: center;
  gap: 40px;
  height: 100%;
  margin-left: 9%;
}


</style>
