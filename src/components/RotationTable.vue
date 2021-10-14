<template>
    <div class="center">
        <table>
            <tr>
                <td>{{player1}}</td>
                <td>{{player2}}</td>
                <td>{{player3}}</td>
            </tr>
            <tr>
                <td>{{player6}}</td>
                <td>{{player5}}</td>
                <td>{{player4}}</td>
            </tr>
        </table>
    </div>
</template>

<script>
export default {
  name: "RotationTable",
  props: {
    player1: String,
    player2: String,
    player3: String,
    player4: String,
    player5: String,
    player6: String,
  },
};
</script>

<style>
    .center {
        display: flex;
        align-items: center;
        justify-content: center;
        height: 5vh;
    }
</style>