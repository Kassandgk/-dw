# -dw
#include <graphics.h>
#include <conio.h>
#include <stdlib.h>
#include <dos.h>
#define R 7
#define MAU YELLOW
#define MAUNEN BLACK
#define CHAM 6

void bong();
void main()
{
	int gdrv = DETECT, gmode, errorcode;
	initgraph(&gdrv, &gmode, "..//BGI");
	errorcode = graphresult();
	if (errorcode != grOk)
	{
		printf("Graphics error : %s\n", gr
