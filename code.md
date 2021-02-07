# PROJECT-ARMY

#include<reg51.h>
sbit  in = P1^2 ;
sbit  relay = P2^0 ;

void delay(unsigned int msec) //Time delay function
{
int i,j ;
for(i=0;i<msec;i++)
  for(j=0;j<1275;j++);
}




void main()
{

while(1)

{
	
	if(in==0)
{
	delay(5);
if(in==0)
{
relay = 0 ;
delay(100);
}
}
	
else
{
relay = 1;
}

}
}
