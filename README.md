//Divide your screen into four region, draw circle, rectangle, ellipse and half ellipse in each region with appropriate message
#include <graphics.h>
#include <stdio.h>
#include <conio.h>
void main()
{
int gd=DETECT,gm;
initgraph(&gd,&gm,"C:\\TURBOC3\\BGI");
int xcen=getmaxx()/2;
int ycen=getmaxy()/2;
line(xcen,0,xcen,getmaxy());
line(0,ycen,getmaxx(),ycen);
circle(xcen/2,ycen/2,100);
rectangle(xcen+50,ycen-200,xcen+200,ycen-50);
ellipse(xcen/2,ycen+ycen/2,0,360,100,50);
ellipse(xcen+xcen/2,ycen+ycen/2,0,180,100,50);
getch();
closegraph();
}


//Draw a simple hut on the screen.

#include <graphics.h>
#include <stdio.h>
#include <conio.h>
void main()
{
int gd=DETECT,gm;
initgraph(&gd,&gm,"C:\\TURBOC3\\BGI");
setcolor(20);
rectangle(150,180,250,300);
rectangle(150,180,420,300);
rectangle(180,250,220,300);
line(200,100,150,180);
line(200,100,250,180);
line(200,100,370,100);
line(370,100,420,180);
getch();
closegraph();
}

