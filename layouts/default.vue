<template>
  <div class="container">
    <div class="row">
      <div class="col-2">
        <AppHeader />
      </div>
      <div class="col-10">
        <div class="container">
          <div class="row">
            <div class="col-8">
              <div class="main">
                <Topbar />
                <nuxt />
              </div>
            </div>
            <div class="col-4">
              <Sidebar />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import AppHeader from '@/components/AppHeader'
import Sidebar from '@/components/Sidebar'
import Topbar from '@/components/Topbar'

export default {
  components: {
    AppHeader,
    Sidebar,
    Topbar
  }
}
</script>
