export default function HomePage() {
  return (
    <div className="min-h-screen bg-white text-brown-800">
      <header className="flex items-center justify-between p-4 shadow-md">
        <img src="/logo.png" alt="Thread Theory Logo" className="h-12" />
        <nav className="space-x-4">
          <a href="/" className="hover:underline">Home</a>
          <a href="/shop" className="hover:underline">Shop</a>
          <a href="/about" className="hover:underline">About</a>
          <a href="/contact" className="hover:underline">Contact</a>
          <a href="/cart" className="hover:underline">Cart</a>
          <a href="/login" className="hover:underline">Login</a>
          <a href="/signup" className="hover:underline">Sign Up</a>
        </nav>
      </header>

      <main className="p-8 text-center">
        <h1 className="text-4xl font-bold mb-4">Welcome to Thread Theory</h1>
        <p className="text-lg mb-6">Customize your hoodie, t-shirt, or jacket in your unique style.</p>
        <a href="/shop" className="inline-block bg-brown-700 text-white px-6 py-2 rounded-xl shadow hover:bg-brown-800">Start Shopping</a>
      </main>

      <section className="p-8">
        <h2 className="text-2xl font-semibold text-center mb-6">Sample Products</h2>
        <div className="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
          {['Hoodie', 'T-Shirt', 'Jacket'].map((item) => (
            <div key={item} className="border rounded-xl p-4 shadow hover:shadow-lg">
              <img src={`/${item.toLowerCase()}.png`} alt={item} className="h-48 w-full object-contain mb-4" />
              <h3 className="text-xl font-medium mb-2">Custom {item}</h3>
              <p className="mb-2">Starting at ₹999</p>
              <a href={`/customize/${item.toLowerCase()}`} className="inline-block bg-brown-700 text-white px-4 py-2 rounded hover:bg-brown-800">Customize</a>
            </div>
          ))}
        </div>
      </section>

      <section className="p-8 text-center">
        <h2 className="text-xl font-semibold mb-4">Track Your Order</h2>
        <form className="max-w-md mx-auto space-y-4">
          <input type="text" placeholder="Enter Order ID" className="w-full border rounded p-2" />
          <button type="submit" className="bg-brown-700 text-white px-4 py-2 rounded hover:bg-brown-800">Track Order</button>
        </form>
      </section>

      <footer className="bg-brown-100 text-center py-4 text-sm mt-10">
        © 2025 Thread Theory. All rights reserved.
      </footer>
    </div>
  );
}
export default function HomePage() { return ( <div className="min-h-screen bg-white text-brown-800"> <header className="flex items-center justify-between p-4 shadow-md"> <img src="/logo.png" alt="Thread Theory Logo" className="h-12" /> <nav className="space-x-4"> <a href="/" className="hover:underline">Home</a> <a href="/shop" className="hover:underline">Shop</a> <a href="/about" className="hover:underline">About</a> <a href="/contact" className="hover:underline">Contact</a> <a href="/cart" className="hover:underline">Cart</a> <a href="/login" className="hover:underline">Login</a> <a href="/signup" className="hover:underline">Sign Up</a> </nav> </header>

<main className="p-8 text-center">
    <h1 className="text-4xl font-bold mb-4">Welcome to Thread Theory</h1>
    <p className="text-lg mb-6">Customize your hoodie, t-shirt, or jacket in your unique style.</p>
    <a href="/shop" className="inline-block bg-brown-700 text-white px-6 py-2 rounded-xl shadow hover:bg-brown-800">Start Shopping</a>
  </main>

  <section className="p-8">
    <h2 className="text-2xl font-semibold text-center mb-6">Sample Products</h2>
    <div className="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
      {['Hoodie', 'T-Shirt', 'Jacket'].map((item) => (
        <div key={item} className="border rounded-xl p-4 shadow hover:shadow-lg">
          <img src={`/${item.toLowerCase()}.png`} alt={item} className="h-48 w-full object-contain mb-4" />
          <h3 className="text-xl font-medium mb-2">Custom {item}</h3>
          <p className="mb-2">Starting at ₹999</p>
          <a href={`/customize/${item.toLowerCase()}`} className="inline-block bg-brown-700 text-white px-4 py-2 rounded hover:bg-brown-800">Customize</a>
        </div>
      ))}
    </div>
  </section>

  <section className="p-8 text-center">
    <h2 className="text-xl font-semibold mb-4">Track Your Order</h2>
    <form className="max-w-md mx-auto space-y-4">
      <input type="text" placeholder="Enter Order ID" className="w-full border rounded p-2" />
      <button type="submit" className="bg-brown-700 text-white px-4 py-2 rounded hover:bg-brown-800">Track Order</button>
    </form>
  </section>

  <footer className="bg-brown-100 text-center py-4 text-sm mt-10">
    © 2025 Thread Theory. All rights reserved.
  </footer>
</div>

); }

