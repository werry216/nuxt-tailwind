<template>
  <div class="font-sans w-full min-h-screen m-0">
    <Header></Header>
    <Dashboard></Dashboard>
    <Content></Content>
    <Footer></Footer>
  </div>
</template>

<script>
//here is the main part of the code
import Header from "~/components/Header";
import Dashboard from "~/components/Dashboard";
import Footer from "~/components/Footer";
import Content from "~/components/Content";
export default {
  components: {
    Header,
    Dashboard,
    Footer,
    Content,
  }
}
</script>
