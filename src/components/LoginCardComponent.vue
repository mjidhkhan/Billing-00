<template>
	<div class="px-8 py-12">
		<div class="px-8 py-12 max-w-md mx-auto sm:max-w-xl  
						lg:min-w-6xl lg:w-1/2 lg:py-24 lg:px-12 ">
			<div class="bg-white pb-4 pt-4 text-center  
						font-semibold text-2xl tracking-wide text-white
						bg-gray-800 shadow-md  rounded rounded-bl-none
						rounded-br-none">
					Login
			</div>
			<div class="bg-white shadow-md rounded rounded-tl-none 
						rounded-tr-none px-12 pt-12
						pb-8 mb-4 flex flex-col ">
				
				<div class="mb-4 mt-4">
					<label 
						class="block text-grey-700 text-sm 
								font-bold mb-2" 
						for="username">
						Username
					</label>
					<input 
						class="shadow appearance-none border rounded 
								w-full py-2 px-3 text-grey-700" 
						id="username" 
						type="text" 
						placeholder="Username">
						
				</div>
				<div class="mb-6">
					<label 
						class="block text-grey-700 text-sm font-bold mb-2" 
						for="password">
						Password
					</label>
					<input 
						class="shadow appearance-none border border-red rounded 
								w-full py-2 px-3 text-grey-700 mb-3" 
						id="password" 
						type="password" 
						placeholder="password">
					
				</div>
				<div class="flex items-center justify-between">
					<button class="bg-gray-700 hover:bg-gray-900 text-white
							focus:outline-none focus:shadow-outline focus:bg-gray-900
							font-bold py-2 px-4 rounded"
						type="button">
						Login
					</button>
					<router-link class="inline-block align-baseline  text-sm text-blue-700 
							hover:text-blue-800" 
							to="passwordreset-request">
						Forgot Password?
					</router-link>
					
				</div>
				<div class="flex items-center justify-end">
					<router-link class="cursor-pointer inline-block align-baseline 
										font-bold text-sm text-blue-700 hover:text-blue-800" 
								to="/register">
							Don't have an account?
					</router-link>
				</div>
			</div>
		</div>
	</div>
</template>


<script>
export default {
	
}
</script>