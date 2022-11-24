<template>
    <div class="container text-center">
      <div class="row row-cols-2">
        <div class="col">
          Info
        </div>
        <div class="col">Statistics</div>
        <div class="col">Column</div>
        <div class="col">Discussion</div>
      </div>
    </div>
</template>

<script>

export default{
    name: "playerinfo",
    props: {
        data: Object
    }
}
</script>
