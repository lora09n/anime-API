# INFO

Hey, This An Anime API ,  Open-Source ,  You Can Use IT For Free !

  # How its work ? 
 
   This build on JSON file u can fetch file on Javasript 


# Code
Html 
<h2>
   <div id="data-anime"></div>
  </h2>

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
      
    ```

       
       Style CSS 
       
       
  .card {
    display: flexbox;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
    max-width: 300px;
    margin: auto;
    text-align: center;
    font-family: arial;
    border-radius: 10px;
    transition: 0.3s;
  }
  
  /* Style the image container */
  .image {
    width: 100%;
    height: 200px;
    background-color: #555;
    border-radius: 10px 10px 0 0;
    overflow: hidden;
    
  }
  /* Style the image */
  .image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: 0.3s;
  }
  
  /* Style the card content */
  .content {
    padding: 10px;
  }
  
  /* Style the card title */
  .title {
    color: whitesmoke;
    font-size: 18px;
  }
  
  /* Style the card description */
  .description {
    color: #bdb2b2;
    font-size: 14px;
  }
  
  /* Style the card button */
  .button {
    border: none;
    outline: none;
    padding: 12px;
    color: white;
    background-color: #000;
    text-align: center;
    cursor: pointer;
    width: 100%;
    font-size: 18px;
    border-radius: 10px;
    transition: 0.3s;
  }
  
  /* Style the hover state of the card */
  .card:hover {
    box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
  }
  
  /* Style the hover state of the image */
  .image:hover img {
    transform: scale(1.1);
  }
  
  /* Style the hover state of the button */
  .button:hover {
    background-color: #555;
  }
  
  /* button */    
  .button-three {
     font-family: 'kurd';
    color:whitesmoke;
      position: relative;
      background-color: #b590ec;
      border: none;
      padding: 20px;
      width: 200px;
      text-align: center;
      -webkit-transition-duration: 0.4s; /* Safari */
      transition-duration: 0.4s;
      text-decoration: none;
      overflow: hidden;
  }
  
  .button-three:hover{
     background:#fff;
     box-shadow:0px 2px 10px 5px #97B1BF;
     color:#000;
  }
  
  .button-three:after {
      content: "";
      background: #b590ec;
      display: block;
      position: absolute;
      padding-top: 300%;
      padding-left: 350%;
      margin-left: -20px !important;
      margin-top: -120%;
      opacity: 0;
      transition: all 0.8s
  }
  
  .button-three:active:after {
      padding: 0;
      margin: 0;
      opacity: 1;
      transition: 0s
  }
  .button-three{
  
    cursor: pointer;
    font-size:24px;
  
  }
  
       </h4>
