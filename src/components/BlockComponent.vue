<template>
    <div class="block">
        <p>{{labelText}} ></p>
    </div>
</template>

<script>

export default {
  name: "BlockComponent", 

  props: {
    labelText: String,
  }
}

</script>

<style scoped lang="css">
.block {
    display: flex;
    width: 190px;
    height: 109px;
    border-radius: 15px;
    background-color: #EFF3F4;
    text-align: center;
    justify-content: center;
    align-items: center;
}
.block:hover {
    background-color: #E7C6C6;
}
</style>