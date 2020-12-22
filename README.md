# 1117
~~~c++
int x=0;
int y=5;
void setup() {
  // put your setup code here, to run once:
  int i;
  for(i=9;i<12;i++)
  pinMode(i,OUTPUT);
}

void loop() {
  // put your main code here, to run repeatedly:
if(x>=255 || x<=0)
  y=-y;
  x=x+y;
  RGB(x,0,0);
  delay(50);
}

void RGB(int r, int g, int b)
{
  analogWrite(9,r);
  analogWrite(10,g);
  analogWrite(11,b);
}
~~~
