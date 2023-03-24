fill(0, 0, 0);
textSize(20);
textAlign(CENTER);

//images of Leafers
var seed= getImage("avatars/leafers-seed");
var seedling= getImage("avatars/leafers-seedling");
var sapling= getImage("avatars/leafers-sapling");
var tree= getImage("avatars/leafers-tree");
var ultimate = getImage("avatars/leafers-ultimate");

var currentScene;

var drawScene1 =function(){
    currentScene = 1;
    background(200, 175, 175);
    image(seed, 50,200);
    text("Leafers started out as a seed",200,50);
};

var drawScene2 =function(){
    currentScene = 2;
    background(146, 217, 235);
    image(seedling, 200,200);
    text("A teenager",200,50);
    text("He read Teen Health book",200,93);
};

var drawScene3 =function(){
    currentScene = 3;
    background(237, 161, 161);
    image(sapling, 200,200);
    text("He went to the Universidy of Maan",200,50);
};

var drawScene4 =function(){
    currentScene = 4;
    background(199, 224, 119);
    image(tree, 200,200);
    text("He got emploid in the University of Chicago" ,200,50);
};

var drawScene5 =function(){
    currentScene = 5;
    background(150, 150, 175);
    image(ultimate, 200,200);
    text("In the end, Leafers became prof. Leafers",200,50);
};

drawScene1();

mouseClicked=function() {
    if (currentScene === 1) {
        drawScene2();
    } else if (currentScene === 2) {
        drawScene3();
    } else if (currentScene === 3) {
        drawScene4();
    } else if (currentScene === 4) {
        drawScene5();
    } else if (currentScene === 5) {
        drawScene1();  
    }
};

