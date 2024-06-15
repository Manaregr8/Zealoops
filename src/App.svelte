<!-- App.svelte -->
<script>
	import Navbar from './components/Navbar.svelte';
	import HomePage from './components/HomePage.svelte';
	import AboutPage from './components/AboutPage.svelte';
  import Footer from "./components/footer.svelte";
  import Product from './components/Product.svelte';
   import Warranty from "./components/warranty.svelte";
	import { Router, Route } from 'svelte-routing';
    import Contact from './components/contact.svelte';
	import Terms from "./components/terms.svelte";
	import Privacy from "./components/privacy.svelte";
	import Return from "./components/return.svelte";
  </script>
  
 
  
  <Router>
	<Navbar />
	<Route path="/" component={HomePage} />
	<Route path="/about" component={AboutPage} />
	<Route path="/product" component={Product} />
	<Route path="/warranty" component={Warranty} />
	<Route path="/terms" component={Terms}/>
	<Route path="/privacy" component={Privacy}/>
	<Route path="/return" component={Return}/>
	<Route path="/contact" component={Contact}/>
	<Footer/>
  </Router>
  <style>     
  </style>
  