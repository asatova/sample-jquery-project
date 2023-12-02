let t1 = new TimelineMax({paused: true});


t1.to(".menu", .8, {
     right: "0%",
     ease: Power4.easeOut,
     transform: 'skewX(0)'
});

//t1.staggerFrom(".menu ul li", .4, {x: -200, opacity: 0, ease:Expo.easeOut}, 0.1);

t1.reverse();
$(document).on("click", ".header-nav__btn", function() {
     t1.reversed(!t1.reversed());
     $('.menu-wrap').addClass('menu-wrap__visible');
});

$(document).on("click", ".menu-close", function() {
     t1.reversed(!t1.reversed());
     setTimeout(function(){$('.menu-wrap').removeClass('menu-wrap__visible')},700);
});


/*const logo = document.querySelectorAll('.preloader-logo path');
 for (let i = 0; i<logo.length; i++) {
 	console.log(`${i} is ${logo[i].getTotalLength()}`);
 }*/

document.body.onload = function() {
setTimeout(function() {
		var preloader = document.querySelector('.preloader');
		if(!preloader.classList.contains('done')) {
			preloader.classList.add('done');
		}
	},3000)
}


 if($(window).width() <= 575.98) {
 	$('.header-nav__btn').attr('src', '/img/menu.svg');

 	window.onscroll = function() {
	    let scrolled = window.pageYOffset || document.documentElement.scrollTop;
	    if(scrolled > 50){
	        $(".header-main").css('top','0');
	        $(".header-main .container").css('background','#D10D0F');
	        $(".header-nav__back .back").css('display', 'none');
	        $(".header-nav__back .top").css('display', 'inline');
	    }
	    if(50 > scrolled){
	        $(".header-main").css('top','20px');   
	        $(".header-main .container").css('background','transparent'); 
	        $(".header-nav__back .top").css('display', 'none');
	        $(".header-nav__back .back").css('display', 'inline');  
	    }
	}

	$(".top").click(function(e) {
		e.preventDefault();
	 	$("html").animate({scrollTop: 0}, 900)
	 });


 }




