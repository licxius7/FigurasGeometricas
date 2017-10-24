# FigurasGeometricas
Area, perímetro de las figuras geométricas.


Figura Ate;
Figura Mariana;
Figura Cuadrado;
Figura Pentagono;
Figura Octagono;
Figura Hexagono;
Figura Triangulo;
Figura Heptagono;
Figura Circulo;
ArrayList <Figura> Figuras;

void setup(){
  Ate= new Triangulo(5,5,5,5,5);
  Mariana= new Cuadrado(7);
  Mariana= new Rectangulo(7,7);
  Mariana= new Pentagono(7);
  Mariana= new Hexagono(7);
  Mariana= new Heptagono(7);
  Mariana= new Octagono(7);
  Mariana= new Circulo(7);
  Figuras = new ArrayList <Figura>();
 Figuras.add(Triangulo);
 Figuras.add(Cuadrado);
 Figuras.add(Pentagono);
 Figuras.add(Hexagono);
 Figuras.add(Heptagono);
 Figuras.add(Octagono);
 Figuras.add(Circulo);
 
 Figuras = new ArrayList <Figura>();
 Figura.add(Triangulo);
 Figura.add(Cuadrado);
 Figura.add(Pentagono);
 Figura.add(Hexagono);
 Figura.add(Heptagono);
 Figura.add(Octagono);
 Figura.add(Circulo);
 /*Figurs = new ArrayList <Figura>();
 Figuras.add(Ate);
 Figuras.add(Mariana);
 */
}

void draw(){
  size(600,800);
  background(0);
  println("Triángulo Perímetro=" + Triangulo.perimetro() + "Área=" + Triangulo.area());
  println("Cuadrado Perímetro=" + Cuadrado.perimetro() + "Área=" + Cuadrado.area());
  println("Rectangulo Perímetro=" + Rectangulo.perimetro() + "Área=" + Rectangulo.area());
  println("Círculo Perímetro=" + Circulo.perimetro() + "Área=" + Circulo.area());   
  println("Pentágono Perímetro=" + Pentagono.perimetro() + "Área=" + Pentagono.area());
  println("Hexágono Perímetro=" + Hexagono.perimetro() + "Área=" + Hexagono.area());
  println("Heptágono Perímetro=" + Heptagono.perimetro() + "Área=" + Heptagono.area());
  println("Octágono Perímetro=" + Octagono.perimetro() + "Área=" + Octagono.area());

 //figuras geometricas
 /*pushMatrix();
 translate(0,0);

 Triangulo.display();
 popMatrix();
 
 pushMatrix();
 translate(0,100);
 Cuadrado.display();
 popMatrix();
 
 pushMatrix();
 translate(0,200);
 Rectangulo.display();
 popMatrix();
 
 pushMatrix();
 translate(0,300);
 Circulo.display();
 popMatrix();
 
 pushMatrix();
 translate(0,400);
 Pentagono.display();
 popMatrix();
 
 pushMatrix();
 translate(0,500);
 Hexagono.display();
 popMatrix();
 
 pushMatrix();
 translate(0,600);
 Heptagono.display();
 popMatrix();
 
 pushMatrix();
 translate(0,700);
 Octagono.display();
 popMatrix();
 */
 println (Ate.perimetro());
 println (Mariana.perimetro());
}

 interface Figura {
  int perimetro();
  float area();
  
  }
  
class Triangulo implements Figura{
  int b,h,l1,l2,l3;
  Triangulo (int b_, int h_, int l1_, int l2_, int l3_){
   b = b_;
   h = h_;
   l1 = l1_;
   l2 = l2_;
   l3 = l3_;
  }
 void display(){
   triangle(5,5,5,5,5,5);
   
 }
  int perimetro(){
    return l1+l2+l3;
  }
  float area(){
    return (b*h)/2;
  } 
 }
class Cuadrado implements Figura{
  int l;
  Cuadrado (int l_){
   l=l_; 
  }
 void display(){
  rect(l,l,l,l); 
   
 }
  int perimetro(){
    return l*4;
  }
  float area(){
    return l*l;
  }
}
class Rectangulo implements Figura{
 int lb,lh;
 Rectangulo (int lb_, int lh_){
  lb = lb_;
  lh = lh_;
 }
 void display(){
   rect(100,100,lb,lh);
   
 }
 int perimetro(){
    return (lb*2)+(lh*2);
 }
 float area(){
   return  lb*lh;
 }
}
class Circulo implements Figura{
 float r;
 Circulo (float r_){
  r = r_;
 }
 void display(){
   ellipse(0,0,r,r);
   
 }
 int perimetro(){
    return round(PI*r)*2; 
 }
 float area(){
   return  (PI*2)*r;
 }
}
class Pentagono implements Figura{
 int l;
 Pentagono (int l_){
  l = l_;
 }
 void display(){
   
   
 }
 int perimetro(){
    return l*5; 
 }
 float area(){
   return  l;
 }
}
class Hexagono implements Figura{
 int l;
 Hexagono (int l_){
  l = l_;
 }
 void display(){
   
   
 }
 int perimetro(){
    return l*6; 
 }
 float area(){
   return  l;
 }
}
class Heptagono implements Figura{
 int l;
 Heptagono (int l_){
  l = l_;
 }
 void display(){
   
   
 }
 int perimetro(){
    return l*7; 
 }
 float area(){
   return  l;
 }
}
class Octagono implements Figura{
 int l;
 Octagono (int l_){
  l = l_;
 }
 void display(){
  
   
 }
 int perimetro(){
    return l*8; 
 }
 float area(){
   return  l;
 }
}
