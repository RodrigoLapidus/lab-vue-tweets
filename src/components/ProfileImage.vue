<template>
    <div>
      <img
      :src="image"
      className="profile"
      alt="profile"
    />
    </div>
  
</template>

<script>
export default {
    name: "ProfileImage",

    props: {
        image: String,
    }

}

</script>

<style>

</style>