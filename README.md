# INFO

Hey, This An Anime API ,  Open-Source ,  You Can Use IT For Free !

  # How its work ? 
 
   This build on JSON file u can fetch file on Javasript 


# Code
Html 

   <h2> <div id="data-anime"></div>  </h2>
  

# JAVASCRIPT 



```


fetch("https://raw.githubusercontent.com/lora09n/anime-API/main/list/isekai/data.json")
.then(function(response){
	return response.json();
})
.then(function(products){
	let placeholder = document.querySelector("#datask");
	let out = "";
	for(let product of products){
		out += `
			 <div class="image"> 
     
    <img src="${product.image}" alt="Card Image"> 
  </div> 
  <div class="content"> 
    <h3 class="title"> 
 ${product.name}
    </h3> 
    <p class="description" > 
${product.description}
 </p> 
    <a href="${product.link}"> 
    <button class="button" id="read-more-button" >More...</button> </a> 
  </div> 
   <br> 
     <br> 
     <br>
		`;
	}
console.log('hey');
	placeholder.innerHTML = out;
});
      
  

 
