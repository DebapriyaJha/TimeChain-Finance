<script>
  // No specific script needed for this static layout
</script>

<style>
  .header-text {
    color: #003A4D; 
    font-size: 2rem; 
  }
  
  .main-content {
    color: black; 
    background-color: white; 
  }

  .header-container {
    margin-left: -1rem;
    padding-left: 2rem; 
  }

  .logo {
    width: 180px; 
    height: auto;
    margin-right: 0.5rem; 
  }

  .main-title {
    font-size: 5rem; 
  }

  .welcome-text {
    font-size: 1.5rem; 
  }

  .description {
    font-size: 2rem; 
    text-align: center; 
  }

  .cta-button {
    font-size: 1.75rem; 
  }

  .register-button:hover {
    background-color: #007A94; 
  }

  .login-button:hover {
    background-color: #4F4F4F; 
  }

  .footer-text {
    font-size: 1.7rem; 
    margin-left: 1rem; 
  }

  .footer-link:hover {
    color: #200889; 
  }

  .footer-link {
    font-size: 1.7rem; 
  }

  .footer-links {
    margin-right: -85rem; 
  }

  .footer-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-left: -1rem;
    padding-left: 2rem; 
  }
</style>

<div class="min-h-screen flex flex-col">
  <header class="bg-white shadow-md">
    <div class="container mx-auto px-4 py-4 flex justify-between items-center header-container">
      <div class="flex items-center">
        <img src="/images/logo.png" alt="Logo" class="logo" />
        <span class="text-xl font-semibold header-text">
          <span class="text-black">TIMECHAIN</span>
          <span class="boldtext-[#003A4D]"> FINANCE</span>
        </span>
      </div>
      <nav class="flex space-x-4">
      </nav>
    </div>
  </header>

  <main class="flex-1 flex flex-col justify-center items-center bg-white text-black py-20 main-content">
    <div class="text-center mb-4">
      <span class="inline-block bg-gray-800 text-sm px-3 py-1 rounded-full mb-2 text-white welcome-text">Welcome to the</span>
      <h1 class="text-5xl font-bold mb-2 main-title">Timechain Finance</h1>
    </div>
    
    <div class="description">
      <p>Your one-stop solution for managing all your financial needs with the power of Web3 technology.</p>
      <p> Explore our platform to learn more and get started. Discover opportunities for borrowing and lending to maximize your financial potential.</p>
    </div>
    
    <div class="flex space-x-4 mt-8">
      <a href="/register" class="bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-700 cta-button register-button">Register</a>
      <a href="/login" class="bg-gray-800 text-white px-4 py-2 rounded hover:bg-gray-700 cta-button login-button">Login</a>
    </div>
  </main>

  <footer class="bg-gray-100 text-gray-600 py-4">
    <div class="container mx-auto px-4 footer-container">
      <p class="footer-text">&copy; 2024 Timechain Finance™. All Rights Reserved.</p>
      <div class="flex space-x-4 footer-links">
        <a href="https://tsoc.vercel.app/" class="text-gray-700 hover:text-gray-900 footer-link">About</a>
        <a href="https://tsoc.vercel.app/" class="text-gray-700 hover:text-gray-900 footer-link">Contact</a>
      </div>
    </div>
  </footer>
</div>
