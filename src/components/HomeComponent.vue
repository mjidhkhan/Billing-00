<template>
<div class="start"> 
	<div  class="antialiased text-gray-800">
		<div class=" flex bg-white overflow-hidden  lg:max-w-full ">
			<div class="px-8 py-12 max-w-md mx-auto sm:max-w-xl 
						lg:max-w-full lg:w-1/2 lg:py-24 lg:px-12 ">
				<div class="xl:max-w-lg xl:ml-auto">
					<img class="h-10" 
						src="/img/logo.svg" 
						alt="Workcation">
					<img class="mt-6 rounded-lg shadow-xl sm:mt-8 sm:h-72 
								sm:w-full sm:object-cover sm:object-center lg:hidden" 
								src="/img/beach-work.jpg" 
								alt="Woman workcationing on the beach">
					<h1 class="mt-2 text-lg font-bold text-gray-800 leading-tight  
								sm:mt-8  sm:text-4xl lg:text-3xl xl:text-4xl">
							You can work from anywhere.
							<br class="sm:hidden lg:inline">
							<span class="text-indigo-500">
								Take advantage of it.
							</span>
					</h1>
					<p class="mt-2 text-gray-600 sm:mt-4 sm:text-xl">
						Workcation helps you find work-friendly rentals in beautiful 
						locations so you can enjoy some nice weather even when you're 
						not on vacation.
					</p>
					<div class="mt-4 sm:mt-6">
						<a href="#" class="btn btn-indigo shadow-lg sm:text-base">
							Book your escape 
						</a>
					</div>
					
				</div>
			</div>
			<div class="hidden lg:block lg:w-1/2 lg:relative 
							sm:bg-gray-100 lg:bg-primary-200 bg-white">
				<img class=" py-12 absolute inset-0  h-full w-full object-cover object-center" 
							src="/img/beach-work.jpg " 
							alt="Woman workcationing on the beach">
			</div>
		</div>
	
		<!-- Destination Card -->
		<div class="max-auto ">
			<div class="bg-gray-100 pb-12 border-gray-200 border-solid border-t">
					<h2 class="text-xl text-gray-800 px-8">Popular destinations</h2>
					<p class="text-gray-600 px-8">
						A selection of great work-friendly 
						cities with lots to see and explore.
					</p>
			</div>
			<div class="flex flex-wrap pb-12">
				<div class="mt-6 w-full px-4 w-1/2 sm:w-1/2 md:w-1/2 lg:w-1/3 xl:w-1/3"  
							v-for="destination in destinations" 
							:key="destination.id" >
						<DestinationCard :destination="destination"/>
					
				</div>
			</div>
		</div>
			<!-- Property Card -->
		<div class="max-auto ">
			<div class="bg-gray-100 pb-12 border-gray-200 border-solid border-t">
					<h2 class="text-xl text-gray-800 px-8">Rentials</h2>
					<p class="text-gray-600 px-8">Available to rent at any time.</p>
			</div>
			<div class="flex flex-wrap pb-12">
				<div class=" items-center justify-center mt-6 w-full 
							px-4 sm:w-1/2 lg:w-1/2 xl:w-1/4 "  
						v-for="property in properties" 
						:key="property.id" >
					<PropertyCard :property="property"/>
				</div>
			</div>
		</div>
	</div>
</div>

</template>

<script>
import DestinationCard from './DestinationCardComponent'
import PropertyCard from './PropertyCardComponent'
import store from '@/data/store'

export default {
	name:'home',
	components: {
		DestinationCard,
		PropertyCard,
	},
  
  data() {
    return {
        destinations:store.PropertyData.popularDestinations ,
        properties:store.PropertyData.popularProperties ,
     }
 },
}
</script>