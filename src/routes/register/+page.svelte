
<nav class="bg-gray-100">
  <div class="max-w-screen-xl p-4">
    <a href="/" class="flex items-center -space-x-6">
      <img src="/images/logo.png" class="h-12" alt="tcf logo" />
      <span class="uppercase text-2xl font-semibold whitespace-nowrap"
        >timechain <span class="text-[#003A4D]">finance</span></span
      >
    </a>
  </div>
</nav>

<section class="bg-gray-100 min-h-11/12 flex flex-col justify-center py-6">
  <h1 class="text-center text-3xl font-bold mb-4 text-gray-800">
    Welcome to Timechain Finance
  </h1>
  <div class="bg-teal-300 container mx-auto max-w-md rounded-2xl shadow-lg p-8">
    <h2 class="text-center mb-8 text-2xl font-semibold text-gray-900">
      Create Your Account
    </h2>
    <form class="space-y-6">
      <div>
        <input
          type="text"
          name="name"
          placeholder="Full Name"
          class="block border border-gray-400 bg-teal-600 w-full text-white p-3 rounded-lg focus:outline-none focus:ring-2 focus:ring-teal-500"
          required
        />
      </div>
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
          id="terms"
          name="terms"
          class="mr-2 text-teal-600 focus:ring-teal-500"
          required
        />
        <label for="terms" class="text-white">
          <!-- svelte-ignore a11y-invalid-attribute -->
          I agree to the <a
            href="#"
            class="text-black underline hover:text-blue-300"
            >Terms and Conditions</a
          >
        </label>
      </div>
      <div>
        <button
          type="submit"
          class="block w-md mx-auto bg-teal-700 hover:bg-teal-600 text-white hover:text-black font-bold py-3 px-4 rounded-lg shadow-md hover:shadow-lg transition-shadow duration-200"
        >
          Create Account
        </button>
      </div>
      <div class="text-gray-700 mt-6 text-center">
        Already have an account?
        <a href="../login/" class="text-blue-500 underline hover:text-blue-700">
          Log in
        </a>.
      </div>
    </form>
  </div>
</section>
