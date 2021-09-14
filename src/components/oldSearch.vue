<template>
  <div class="container">
    <ul class="list-group text-left">
      <li class="list-group-item">
        <div>
          <strong></strong>
        </div>
        <br />
        <div>
          <strong class="text-success"></strong>
          <span class="text-info"></span>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  setup() {},
  mounted() {
    axios
      .get("https://api.collectapi.com/health/dutyPharmacy?&il=Bursa", {
        headers: {
          Authorization: "apikey 0SqN7rZI2rmDGyfMrWGuS9:26EubLZxIVmmf1lOEiYWCs",
          Content: "text/plain; charset=utf-8",
        },
      })
      .then((ecz) => {
        console.log(ecz.data);
        this.ecz = ecz.data.result;
      })
      .catch((error) => {
        console.error(error);
      });
  },
};
</script>

<style scoped>
</style>