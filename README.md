Controller
==========

1. Controller UI with X Y commands in a range of -1 to 1.
1. Portrait one handed "binary" view and landscape two handed granular view
1. Touch support only. No mouse support.
1. Tested in Android Chrome and iOS Safari

#To use

To use create a new instance of controller and assign a function to onChange; then call the start method. Your function could trigger a socket.io event or manipulate another element on the screen.

#Example


    var controller = new Controller();
    controller.onChange = function(data){
        console.log(data.x, data.y);
    };
    controller.start();

    //0,0
    //-1,1
    //1,-1
    //0.96,-0.23
