<template>
  <div class="home">
    <Navbar v-model="isSidebarOpen"/>
    <Sidebar :active="isSidebarOpen"/>
    <Header />
    <Teams />
    <Work />
    <Hire />
    <Create />
    <Join />
    <Templates />
    <Review />
    <Start />
    <Footer />
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Sidebar from '@/components/Sidebar.vue'
import Header from '@/components/Header.vue'
import Teams from '@/components/Teams.vue'
import Work from '@/components/Work.vue'
import Button from '@/components/Button.vue'
import Hire from '@/components/Hire.vue'
import Create from '@/components/Create.vue'
import Join from '@/components/Join.vue'
import Templates from '@/components/Templates.vue'
import Review from '@/components/Review.vue'
import Start from '@/components/Start.vue'
import Footer from '@/components/Footer.vue'

export default {
  components: { Navbar, Sidebar, Header, Teams, Work, Button, Hire, Create, Join, Templates, Review, Start, Footer },
  name: 'HomeView',
  data() {
    return {
      isSidebarOpen: false,
    }
  }
}
</script>
