//glabal variables
var myarray

//Bubble constructor
function Bubble(){;
// create x and y properties (variables)                  
    this.x = random(width);
    this.y = random(height);
    this.r = 20; //r is for trhe radius which is 1/2 the width of the circle
   this.bubbleSize = this.r*2;//width anf height are twice the radius               

//method:draw the buble
this.drawBubble = function(){
ellipse(this.x,this.y,this.bubbleSize,this.bubbleSiz);)
}
}//end Bubble

function setup(){
//create the canvas. put into a variable to assocaite with a element
var cnv = createCanvas(windowWidth,windowHeight);
cnv.parent("windows");
     
    // add stuff to the array with a loop
    for(var i =0; i<10; i++){
        //add Bubbles to the array
        myArray[i] = new Bubble();
        myArray[i].drawBubble();
    }
} //end setup
    
//listen to mouse pressed with the built in p5 mousePressed method
    function mousePressed(){
        //check that this is working
        console.log("mouse Pressed");
    }
    //loop through myArray and check if mouse is in each Bubbble
    for(var i=0; i < myArray.length; i++){
    myArray[i].x myArray[i].r
    }
}//end mousePressed
