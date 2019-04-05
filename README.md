let y = 10;

function setup() {
  createCanvas(720, 500); // eerste stap
  stroke(158); // Dit geeft de lijn aan die van boven naar beneden gaat = lijn is wit
  frameRate(50); //de snelheid van de lijn die beweegt
  bg = loadImage('zonnebloem.jpg');
}

function draw() {
  background(bg); // achtergrond is foto
  y = y - 1;
  if (y < 0) {
    y = height;
  }
  line(0, y, width, y);
  text("Yoek,dit is een 10 waard. Yoek,dit is een 10 waard. Yoek,dit is een 10 waard. Yoek, dit is een 10 waard",0,y) //dit is de tekst op de lijn
  textSize(15) //dit geeft de groote van de tekst aan op de lijn
  textStyle(BOLDITALIC) //dit is de lettertype
ellipseMode(RADIUS); // zet ellipseMode to RADIUS
fill(255); // de vulling is in de kleur wit
ellipse(100, 50, 3, 3); // een getekende rondje die de ster moet voorstellen ookal is de lucht blauw
  ellipse(200, 70, 3, 3);
  ellipse(300, 30, 3, 3);
  ellipse(350, 40, 3, 3);
  ellipse(400, 15, 3, 3);
  
  if (mouseIsPressed) {
    ellipse(50, 50, 50, 50); // dit stelt de zon voor die de bloem laat bloeien
  } else {
    ellipse(25, 25, 50, 50);
  }
