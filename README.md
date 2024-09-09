# my-e-commerce-store
// src/Home.js
import React from 'react';

function Home() {
  return (
    <div>
      <h1>Welcome to My Ecommerce Store!</h1>
      <p>This is the home page.</p>
      <div>
        <h2>New Arrivals</h2>
        <ul>
          <li>T-SHIRT SAN</li>
          <li>T-SHIRT BICSAN</li>
          <li>T-SHIRT BESTIE</li>
        </ul>
      </div>
    </div>
  );
}

export default Home;

// src/Products.js
import React from 'react';

function Products() {
  const products = [
    { id: 1, name: 'T-SHIRT SAN', price: 29.99 },
    { id: 2, name: 'T-SHIRT BICSAN', price: 39.99 },
    { id: 3, name: 'T-SHIRT BESTIE', price: 49.99 },
  ];

  return (
    <div>
      <h1>Products</h1>
      <ul>
        {products.map((product) => (
          <li key={product.id}>
            {product.name} - ${product.price}
          </li>
        ))}
      </ul>
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
      <div>
        <h2>Contact Information: 0792076256</h2>
        <p>Email: AFRICAPASTUNVEILED@GMAIL.com</p>
        <p>Phone: +254 792076256</p>
      </div>
    </div>
  );
}

export default About;
