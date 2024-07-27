 <section class="bg-[#FFCE00] dark:bg-gray-900">
    <div class="py-8 px-4 mx-auto max-w-screen-xl lg:py-16 lg:px-12">
      <div class="flex flex-col lg:flex-row justify-between items-center">
        <div class="lg:w-1/2 mb-8 lg:mb-0">
          <h1 class="mb-4 text-4xl font-extrabold tracking-tight leading-none text-gray-900 md:text-5xl lg:text-6xl dark:text-white">Get Loan For Your Business Growth or Startup</h1>
          <p class="mb-8 text-lg font-normal text-gray-700 lg:text-xl dark:text-gray-400">Apply for loan in minutes</p>
        </div>
        <div class="lg:w-1/2">
          <div class="bg-white p-8 rounded-lg shadow-md dark:bg-gray-800">
            <h3 class="text-2xl font-bold mb-6 text-gray-900 dark:text-white">How much do you need</h3>
            <form>
              <div class="mb-4">
                <label for="amount" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Loan Amount:</label>
                <input type="text" id="amount" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
              </div>
              <div class="mb-4">
                <label for="duration" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Duration:</label>
                <input type="text" id="duration" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
              </div>
              <div class="mb-4">
                <label for="purpose" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Purpose:</label>
                <input type="text" id="purpose" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
              </div>
              <div class="grid grid-cols-2 gap-4 mb-4">
                <div>
                  <label for="name" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Name:</label>
                  <input type="text" id="name" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
                </div>
                <div>
                  <label for="phone" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Phone:</label>
                  <input type="text" id="phone" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
                </div>
              </div>
              <button type="submit" class="w-full text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Get Your Loan Now!</button>
            </form>
          </div>
        </div>
      </div>
    </div>
  </section>
  
  <style>
    .loan-item {
      transition: all 0.3s ease;
    }
    .loan-item:hover .loan-details {
      transform: translateY(0);
    }
    .loan-details {
      transition: all 0.3s ease;
      transform: translateY(calc(100% - 4rem)); /* Adjust based on your title height */
    }
    .find-out-more {
      color: white;
      text-decoration: underline;
      text-decoration-color: blue;
      text-decoration-thickness: 2px;
      text-underline-offset: 4px;
    }
  </style>
  
  <section class="bg-white dark:bg-gray-900 py-16">
    <div class="container mx-auto px-4">
      <div class="text-center mb-12">
        <h2 class="text-3xl font-bold text-gray-900 dark:text-white mb-4">Funding Opportunities</h2>
      </div>
      <div class="flex flex-nowrap h-96">
        {#each [
          { title: "Personal Loan", image: "/personal-loan.jpg" },
          { title: "Business Loan", image: "/business-loan.webp" },
          { title: "Education Loan", image: "/education-loan.jpg" },
          { title: "Commercial Loan", image: "/commercial-loan.jpg" },
          { title: "Health Loan", image: "/medical-loan.jpg" }
        ] as loan, index}
          <div class="flex-1 relative overflow-hidden loan-item">
            <div class="absolute inset-0 bg-blue-900 bg-opacity-60"></div>
            <img src={loan.image} alt={loan.title} class="w-full h-full object-cover" />
            <div class="loan-details absolute inset-x-0 bottom-0 p-4 text-white">
              <h4 class="text-white text-2xl font-bold mb-4">
                <span class="text-blue-300">{(index + 1).toString().padStart(2, '0')}.</span> {loan.title}
              </h4>
              <p class="mb-4">But that's not the kind of attention you want, is it?</p>
              <a href="#" class="find-out-more hover:text-blue-300">Find Out More</a>
            </div>
          </div>
        {/each}
      </div>
    </div>
  </section>


  <section class="bg-white dark:bg-gray-900 py-16">
    <!-- Previous Funding Opportunities section code here -->
  </section>
  
  <section style="background-color: #f3f4f6; padding: 4rem 0;">
    <div style="max-width: 1200px; margin: 0 auto; padding: 0 1rem;">
      <h2 style="font-size: 2.5rem; font-weight: bold; text-align: center; margin-bottom: 2rem; color: #1f2937;">Loan Request Process</h2>
      
      <div style="display: flex; flex-wrap: wrap; justify-content: space-between;">
        <div style="width: calc(20% - 1rem); background-color: white; border-radius: 0.5rem; padding: 1.5rem; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); margin-bottom: 1rem;">
          <h3 style="font-size: 1.25rem; font-weight: bold; margin-bottom: 1rem; color: #4b5563;">1. Browse Requests</h3>
          <p style="font-size: 1rem; color: #6b7280;">User can browse loan requests by category, amount, interest rate, and borrower rating.</p>
        </div>
        
        <div style="width: calc(20% - 1rem); background-color: white; border-radius: 0.5rem; padding: 1.5rem; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); margin-bottom: 1rem;">
          <h3 style="font-size: 1.25rem; font-weight: bold; margin-bottom: 1rem; color: #4b5563;">2. View Details</h3>
          <p style="font-size: 1rem; color: #6b7280;">User selects a loan request to view detailed information.</p>
        </div>
        
        <div style="width: calc(20% - 1rem); background-color: white; border-radius: 0.5rem; padding: 1.5rem; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); margin-bottom: 1rem;">
          <h3 style="font-size: 1.25rem; font-weight: bold; margin-bottom: 1rem; color: #4b5563;">3. Fund Loan</h3>
          <p style="font-size: 1rem; color: #6b7280;">User clicks "Fund Loan" and enters the amount they wish to lend.</p>
        </div>
        
        <div style="width: calc(20% - 1rem); background-color: white; border-radius: 0.5rem; padding: 1.5rem; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); margin-bottom: 1rem;">
          <h3 style="font-size: 1.25rem; font-weight: bold; margin-bottom: 1rem; color: #4b5563;">4. Confirm Terms</h3>
          <p style="font-size: 1rem; color: #6b7280;">User reviews the loan terms and confirms the funding.</p>
        </div>
        
        <div style="width: calc(20% - 1rem); background-color: white; border-radius: 0.5rem; padding: 1.5rem; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); margin-bottom: 1rem;">
          <h3 style="font-size: 1.25rem; font-weight: bold; margin-bottom: 1rem; color: #4b5563;">5. Transfer Funds</h3>
          <p style="font-size: 1rem; color: #6b7280;">Funds are transferred to the borrower's account and recorded on the blockchain.</p>
        </div>
      </div>
    </div>
  </section>
