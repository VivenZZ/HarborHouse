<template>
  <div id="test">
    <HeaderIndex :headerInfo='headerInfo' />
  </div>
</template>
<script>
import HeaderIndex from '@/components/libs/header'
export default{
  name: 'Test',
  components: {
    HeaderIndex
  },
  data () {
    return {
      headerInfo: [
        {
          id: 1
        },
        {
          id: 2
        },
        {
          id: 3
        }
      ]
    }
  }
}
</script>
