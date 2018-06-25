<template>
  <div id="root">
    <Quotebar />
    <Bio :info="info"/>
    <Showcase />
    <Tech title="What I'm working with"/>
    <SocialBar :social="info.socialAccounts" />
    <Footer />
  </div>
</template>

<script>
import info from '@/data/info'
import Quotebar from '@/components/Quotebar'
import Bio from '@/components/Bio'
import Showcase from '@/components/Showcase'
import Tech from '@/components/Tech'
import SocialBar from '@/components/SocialBar'
import Footer from '@/components/Footer'
export default {
  components: {
    Quotebar,
    Bio,
    Showcase,
    Tech,
    SocialBar,
    Footer
  },
  data () {
    return {
      info
    }
  }
}
</script>

<style>
  body {
    font-family: 'Roboto', sans-serif;
    font-size: 18px;
    color: #525f7f;
  }
  section {
    padding: 100px 0;
  }
  h1,
  h2,
  h3,
  h4 {
    font-weight: 700;
  }
</style>
