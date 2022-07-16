"use strict"

function ibg(){

	let ibg = document.querySelectorAll(".ibg");
	for (var i = 0; i < ibg.length; i++) {
		if(ibg[i].querySelector('img')){
			ibg[i].style.backgroundImage = 'url('+ibg[i].querySelector('img').getAttribute('src')+')';
		}
	}
}

ibg();

let body = document.querySelector('body');
let menu = document.querySelector('.header__menu');
let burger = document.querySelector('.header__icon');
let menuLinks = document.querySelectorAll('.menu__link');



burger.addEventListener('click', function(e){
	menu.classList.toggle('_active');
	burger.classList.toggle('_active');
	body.classList.toggle('_lock');
});



menuLinks.forEach(menuLink => menuLink.addEventListener('click', function(e){
	menu.classList.remove('_active');
	body.classList.remove('_lock');
}));


let today = new Date();
let day = today.getDate(); 
let month = today.getMonth(); 
let year = today.getFullYear(); 
console.log(day);
console.log(month);
console.log(year);

if(month < 10){
	month = '0' + month;
}

document.querySelector('.calendar1').value = `${year}-${month}-${day + 1}`;

document.querySelector('.calendar2').value = `${year}-${month}-${day + 7}`;





let mainPopupButton = document.querySelector('.mainscreen__button');
let popup = document.querySelector('.popup');
let popupIcon = document.querySelector('.popup__icon');

mainPopupButton.addEventListener('click', function(e){
	popup.classList.toggle('_active');
	body.classList.add('_lock');
})

popupIcon.addEventListener('click', function(e){
	popup.classList.remove('_active');
	body.classList.remove('_lock');
})
