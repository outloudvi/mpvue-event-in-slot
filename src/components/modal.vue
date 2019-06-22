<template>
    <div>
        <div class="test a1"  @click="methodsInModel">
          Here is out of slot
        </div>
        <div class="testa a2">
            <slot></slot>
        </div>
    </div>
</template>

<script>
export default {
  props: [""],
  methods: {
    methodsInModel: function() {
      console.log("Component methods out of slot")
    }
  }
};
</script>

<style scoped>
.test {
  height: 30px;
}

.a1 {
  background: red;
}

.a2 {
  background: cadetblue;
}
</style>
