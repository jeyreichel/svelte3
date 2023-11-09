<script>
  import { Router, Route } from "svelte-routing";
  import Header from "./Components/Header.svelte";
  import Notice from "./Components/Notice.svelte";
  import Footer from "./Components/Footer.svelte";
  import Loader from "./Components/Loader.svelte";
  import Home from "./routes/home/home.svelte";
  import About from "./routes/about/about.svelte";
  import Contact from "./routes/contact/contact.svelte";
  import DedicatedServer from "./routes/dedicated-server/dedicated-server.svelte";
  import ResellerHosting from "./routes/reseller-hosting/reseller-hosting.svelte";
  import SharedHosting from "./routes/shared-hosting/shared-hosting.svelte";
  import Testimonials from "./routes/testimonials/testimonials.svelte";
  import VpsHosting from "./routes/vps-hosting/vps-hosting.svelte";

  export let url = "";
</script>

<div class="app">
  <div class="body-overlay" />
  <button class="scrolltop-btn"><i class="fa-solid fa-angle-up" /></button>

  <Loader />

  <Router {url}>
    <div class="main-wrapper">
      <Notice />
      <Header />

      <main>
        <Route path="/"><Home /></Route>
        <Route path="/home"><Home /></Route>
        <Route path="/about"><About /></Route>
        <Route path="/contact"><Contact /></Route>
        <Route path="/dedicated-server"><DedicatedServer /></Route>
        <Route path="/reseller-hosting"><ResellerHosting /></Route>
        <Route path="/shared-hosting"><SharedHosting /></Route>
        <Route path="/testimonials"><Testimonials /></Route>
        <Route path="/vps-hosting"><VpsHosting /></Route>
      </main>
      <Footer />
    </div>
  </Router>
</div>
