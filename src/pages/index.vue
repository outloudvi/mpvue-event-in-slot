<template>
  <div>
    <modal>
      <div @click="methodsInSlot">
        Here is slot
      </div>
    </modal>
  </div>
</template>

<script>
import modal from "@/components/modal";

export default {
  components: {
    modal
  },
  methods: {
    methodsInSlot: function() {
      console.log("Page methods inside slot")
    }
  }
};
</script>

<style scoped>

</style>

