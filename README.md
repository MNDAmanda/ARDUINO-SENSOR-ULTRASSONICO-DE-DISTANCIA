# cod-sensor-de-proximidade
#define	a	7
#define	b	8
#define	c	9
#define	d	10
#define	e	11
#define	f	12
#define	g	13
#define	a2	0
#define	b2	1
#define	c2	2
#define	d2	3
#define	e2	4
#define	f2	5
#define	g2	6

int matriz[10][7]={
//   a,b,c,d,e,f,g  
    {1,1,1,1,1,1,0},//0
    {0,1,1,0,0,0,0},//1
    {1,1,0,1,1,0,1},//2
    {1,1,1,1,0,0,1},//3
    {0,1,1,0,0,1,1},//4
    {1,0,1,1,0,1,1},//5
    {1,0,1,1,1,1,1},//6
    {1,1,1,0,0,0,0},//7
    {1,1,1,1,1,1,1},//8
    {1,1,1,0,0,1,1},//9
};

void setup()
{
  pinMode(a, OUTPUT);
  pinMode(b, OUTPUT);
  pinMode(c, OUTPUT);
  pinMode(d, OUTPUT);
  pinMode(e, OUTPUT);
  pinMode(f, OUTPUT);
  pinMode(g, OUTPUT);
  pinMode(a2, OUTPUT);
  pinMode(b2, OUTPUT);
  pinMode(c2, OUTPUT);
  pinMode(d2, OUTPUT);
  pinMode(e2, OUTPUT);
  pinMode(f2, OUTPUT);
  pinMode(g2, OUTPUT);
}

void loop()
{
  
  for (int j=0; j<10; j++){
    digitalWrite(a,matriz[j][0]);
    digitalWrite(b,matriz[j][1]);
    digitalWrite(c,matriz[j][2]);
    digitalWrite(d,matriz[j][3]);
    digitalWrite(e,matriz[j][4]);
    digitalWrite(f,matriz[j][5]);
    digitalWrite(g,matriz[j][6]);
    digitalWrite(a2,matriz[0][0]);
    digitalWrite(b2,matriz[0][1]);
    digitalWrite(c2,matriz[0][2]);
    digitalWrite(d2,matriz[0][3]);
    digitalWrite(e2,matriz[0][4]);
    digitalWrite(f2,matriz[0][5]);
    digitalWrite(g2,matriz[0][6]); 
    delay(100);
      for(int i=1; i<10; i++){
        digitalWrite(a2,matriz[i][0]);
        digitalWrite(b2,matriz[i][1]);
        digitalWrite(c2,matriz[i][2]);
        digitalWrite(d2,matriz[i][3]);
        digitalWrite(e2,matriz[i][4]);
        digitalWrite(f2,matriz[i][5]);
        digitalWrite(g2,matriz[i][6]); 
        delay(100);
      }
    }
}
