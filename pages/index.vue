<template>
<div>
  <Navbar/>
  <Home/>
</div>
</template>

<script>
export default {
   head() {
      return {
        title: this.title,
        meta: [
          // hid is used as unique identifier. 
          {
            hid: 'Description',
            name: 'Description',
            content: 'home page'
          }
        ]
      }
    }
}
</script>
