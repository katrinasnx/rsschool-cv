# Katsiaryna Hubenka
## Contact Information
GitHub: [katrinasnx](https://github.com/katrinasnx)  
Email: katiahubenka@gmail.com
***
## About me
Software Engineering student. I like maths, computer science, fashion and chess. Open to new opportunities and cooperation in interesting projects.
***
## Skills
Languages: JavaScript, C#, HTML5, CSS, PHP, SQL  
Web Development: OOP, DOM Manipulation, REST APIs (Fetch), Node.js  
Tools: Git, GitHub, MySQL, MarkDown
***
## Projects
__[Web Application](https://katrinasnx.github.io/weather-app/)__  
Tic-Tac-Toe Game  
Age calculator  
Countdown to New Year
*** 
## My code 
```javascript 
    const btn = document.querySelector("button");

    btn.addEventListener("click", async () => {
    const city = document.querySelector("#input");
	let url = `https://api.openweathermap.org/data/2.5/weather?q=${city.value}&appid=b954a42e05bdf09d9446a6c867191ebb`;
	try {
		const resp = await fetch(url);
		const data = await resp.json();
		document.querySelector(".weatherDiv").innerHTML = `
        <div class="weather">
        <img src="http://openweathermap.org/img/w/${data.weather[0].icon}.png" width="100"/>
        <div class="text">
        <h4>City: ${data.name}</h4>
        <h5>Temperature: ${Math.round(data.main.temp - 273.15)}°C </h5>
        <h5>Description: ${data.weather[0].description}</h5>
        </div>
        </div>`;
		const divContainer = document.querySelector(".container");
		divContainer.style.height = "350px";
		city.value = '';
	} catch (error) {
		console.log(error);
	}
}); 
```
***
## Education
Technical High School Complex No.2 – *Katowice Software Developer (Technik Programista)* | 09.2024 – Present
*** 
## Langueges
__Polish__: B2  
__Russian__: Native  
__English__: B2  
