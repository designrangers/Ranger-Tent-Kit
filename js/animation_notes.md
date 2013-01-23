//BASICS FOR TWEEN LITE

// TweenLite.to( [target object], [duration in seconds], [destination values] )

// TweenLite.from

//or use the object-oriented syntax...
//var tween = new TweenLite(element, 1, {css:{width:"50%"}});

/*
Select multiple vars 
eg: TweenLite.to([red, yellow, green], 1, {css:{opacity:0.3}});
or: TweenLite.to($(".box"), 1, {css:{opacity:0.3}});
*/

/*
NOTE ~ Remove the ( - ) for css properties and instead use camelCase.
eg: backgroundColor:"black"
or: borderBottomColor:"#90e500"
*/

// Increments use += or -= like ( left:"+=100px" )

// Callbacks: onStart, onUpdate, onComplete, onReverse, onReverseComplete

/*
$(document).ready(function() {

	var logo = $(".logo");
    TweenLite.from(logo, 1, {css:{left:"0", opacity:0}, delay:1, ease:Power4.easeOut});

});
*/


/*
$(document).ready(function() {

	var logo = $(".logo");
	var btn = $(".increment");

	btn.click(function() {
    	
    	var tween = TweenLite.to(logo, 1, {css:{left:"-=100px"}, ease:Power4.easeOut, onComplete:completeHandler});

    	function completeHandler() {
    		window.alert("Animation Complete");
    	}

	});
});
*/

/*
$(document).ready(function() {

	var logo = $(".logo");
	var btn = $(".increment");
	var restartBTN = $(".restart");

    //var tween = TweenLite.to(logo, 1, {css:{left:"100px"}, ease:Power4.easeOut});

    $(btn).click(function(){

    	var tween = TweenLite.to(logo, 1, {css:{left:"-=100px"}, ease:Power4.easeOut});

	    $(restartBTN).click(function(){
	    	tween.restart();
	    });

    });

});
*/

//pause the tween initially
//var myTween = new TweenLite(photo, 1.5, {width:100, paused:true});
 
//then later, resume
//myTween.resume();

