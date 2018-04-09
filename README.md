void setup(){
  size(300,900);
  background(0);
}
int x= 0;
int y= 0;
int spacing = 6;


void draw() {
 stroke(random(255), random(206) ,random(104));
 if (random(1) < 0.5) {
    
      line(x, y, x+spacing, y+spacing);
 } else {
      rect(x, y+2, x+2, 2);  
      line(x, y+spacing, x+spacing, y);  
}
x = x + spacing;
if (x > width) {
  x = 0;
  y = y + spacing *2;
}
}
