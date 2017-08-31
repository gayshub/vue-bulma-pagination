<template>
  .....
  
  <nav class="pagination is-right " role="navigation" aria-label="pagination" style="padding-right: 15px">
			<ul class="pagination-list" >
				<div>
					<li><a class="pagination-link" aria-label="Goto page 1" @click="getLinodeData(1)"><</a></li>
				</div>
				<div v-for="(n,index) in totalPages">
					<li><a class="pagination-link" :class="{ 'is-current': index+1 === currentPage }" @click="getLinodeData(index+1)">{{ n }}</a></li>
				</div>
				<div>
					<li><a class="pagination-link" aria-label="Goto " @click="getLinodeData(totalPages)">></a></li>
				</div>
			</ul>
		</nav>
    
    ....
 </template>
