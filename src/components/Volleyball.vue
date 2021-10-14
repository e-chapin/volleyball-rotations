<template>
    <div>
        <label for="player1">Player 1 </label>
        <input v-model="player1"/>
        <br/><br/>
        <label for="player2">Player 2 </label>
        <input type="text" v-model="player2"/>
        <br/><br/>
        <label for="player3">Player 3 </label>
        <input type="text" v-model="player3"/>
        <br/><br/>
        <label for="player4">Player 4 </label>
        <input type="text" v-model="player4"/>
        <br/><br/>
        <label for="player5">Player 5 </label>
        <input type="text" v-model="player5"/>
        <br/><br/>
        <label for="player6">Player 6 </label>
        <input type="text" v-model="player6"/>
        <hr/>
        <RotationTable v-bind="{ player1: player1, player2: player2, player3: player3, player4: player4, player5: player5, player6: player6 }"/>
        <RotationTable v-bind="{ player1: player6, player2: player1, player3: player2, player4: player3, player5: player4, player6: player5 }"/>
        <RotationTable v-bind="{ player1: player5, player2: player6, player3: player1, player4: player2, player5: player3, player6: player4 }"/>
        <RotationTable v-bind="{ player1: player4, player2: player5, player3: player6, player4: player1, player5: player2, player6: player3 }"/>
        <RotationTable v-bind="{ player1: player3, player2: player4, player3: player5, player4: player6, player5: player1, player6: player2 }"/>
        <RotationTable v-bind="{ player1: player2, player2: player3, player3: player4, player4: player5, player5: player6, player6: player1 }"/>

    </div>
</template>

<script>
import RotationTable from "./RotationTable.vue";
export default {
  name: "Volleyball",
  components: {
    RotationTable 
  },
  data () {
      return {'player1': '', 'player2': '', 'player3': '', 'player4': '', 'player5': '', 'player6': ''}
    }
};
</script>