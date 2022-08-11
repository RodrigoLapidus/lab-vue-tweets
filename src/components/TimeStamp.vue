<template>
  <div>
    <span className="timestamp">{{ time }}</span>
  </div>
</template>

<script>
export default {
    name: "TimeStamp",

    props: {
        time: String,
    }

}
</script>

<style>

</style>