<section class="bg-gray-100 min-h-screen flex flex-col justify-center py-6">
    <h1 class="text-center text-3xl font-bold mb-4 text-gray-800">Welcome Back!</h1>
    <div class="bg-teal-300 container mx-auto max-w-md rounded-2xl shadow-lg p-8">
      <h2 class="text-center mb-8 text-2xl font-semibold text-gray-900">Log In</h2>
      <form class="space-y-6">
        <div>
          <input
            type="email"
            name="email"
            placeholder="Email"
            class="block border border-gray-400 bg-teal-600 w-full text-white p-3 rounded-lg focus:outline-none focus:ring-2 focus:ring-teal-500"
            required
          />
        </div>
        <div>
          <input
            type="password"
            name="password"
            placeholder="Password"
            class="block border border-gray-400 bg-teal-600 w-full text-white p-3 rounded-lg focus:outline-none focus:ring-2 focus:ring-teal-500"
            required
          />
        </div>
        <div class="flex items-center">
          <input
            type="checkbox"
            id="remember"
            name="remember"
            class="mr-2 text-teal-600 focus:ring-teal-500"
          />
          <label for="remember" class="text-white">
            Remember me
          </label>
        </div>
        <div>
          <button
            type="submit"
            class="block w-md mx-auto bg-teal-700 hover:bg-teal-600 text-white hover:text-black text-xl font-bold py-4 px-8 rounded-lg shadow-md hover:shadow-lg transition-shadow duration-200"
          >
            Log In
          </button>
        </div>
      </form>
    </div>
    <div class="text-gray-700 mt-6 text-center">
      Don't have an account? 
      <a href="../register/" class="text-blue-500 underline hover:text-blue-700">
        Sign Up
      </a>.
    </div>
  </section>