<template>
  <div class="home">
    <Content />
  </div>
</template>

<script>
// @ is an alias to /src
import Content from '@/components/home/HomeContent'

export default {
  name: 'home',
  components: {
    Content
  }
}
</script>
