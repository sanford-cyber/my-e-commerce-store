# my-e-commerce-store
// src/App.js
import React from 'react';
import { BrowserRouter as Router, Route, Switch } from 'react-router-dom';
import Navigation from './Navigation';
import Home from './Home';
import Products from './Products';
import About from './About';

function App() {
  return (
    <Router>
      <Navigation />
      <Switch>
        <Route exact path="/" component={Home} />
        <Route path="/products" component={Products} />
        <Route path="/about" component={About} />
      </Switch>
    </Router>
  );
}

export default App;

// src/Navigation.js
import React from 'react';
import { Link } from 'react-router-dom';

function Navigation() {
  return (
    <nav>
      <ul>
        <li><Link to="/">Home</Link></li>
        <li><Link to="/products">Products</Link></li>
        <li><Link to="/about">About</Link></li>
      </ul>
    </nav>
  );
}

export default Navigation;

// src/Home.js
import React from 'react';

function Home() {
  return (
    <div>
      <h1>Welcome to My Ecommerce Store!</h1>
      <p>This is the home page.</p>
    </div>
  );
}

export default Home;

// src/Products.js
import React from 'react';

function Products() {
  return (
    <div>
      <h1>Products</h1>
      <p>This is the products page.</p>
    </div>
  );
}

export default Products;

// src/About.js
import React from 'react';

function About() {
  return (
    <div>
      <h1>About</h1>
      <p>This is the about page.</p>
    </div>
  );
}

export default About;
