<script>
    import Herobanner from "./herobanner.svelte";
    import Secondsection from "./secondsection.svelte";
    import Specs from "./specs.svelte";
    import Accessories from "./accessories.svelte";
    import Testimonial from "./testimonial.svelte";
    import Thirdsection from "./thirdsection.svelte";
    import Product from './Product.svelte';
	import { Router, Route } from 'svelte-routing';

  </script>
  
 
  
  <Router>
    <Herobanner/>
	<Route path="/product" component={Product} />
  </Router>

<Secondsection />
<Thirdsection />
<Accessories/>
<Specs />
<Testimonial/>