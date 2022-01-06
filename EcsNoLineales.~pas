unit EcsNoLineales;

interface

uses
  Windows, Messages, SysUtils, Variants, Classes, Graphics, Controls, Forms,
  Dialogs, StdCtrls, jpeg, ExtCtrls;

type
  TForm1 = class(TForm)
    Label1: TLabel;
    Image1: TImage;
    Label2: TLabel;
    x1: TEdit;
    x2: TEdit;
    x3: TEdit;
    x4: TEdit;
    Label3: TLabel;
    Label4: TLabel;
    Label5: TLabel;
    Label6: TLabel;
    Btn1: TButton;
    repet: TEdit;
    Label7: TLabel;
    Label8: TLabel;
    Label9: TLabel;
    Label10: TLabel;
    Label11: TLabel;
    f01: TEdit;
    f02: TEdit;
    f03: TEdit;
    f04: TEdit;
    procedure Btn1Click(Sender: TObject);
    procedure FormCreate(Sender: TObject);
  private
    { Private declarations }
  public
    { Public declarations }
  end;

var
  Form1: TForm1;
  repeticiones,itera: integer;
  pi,e: real;

  x01,x02,x03,x04,f1,f2,f3,f4,h1,h2,h3,h4: real;

  d00,d01,d02,d03:real;
  d10,d11,d12,d13:real;
  d20,d21,d22,d23:real;
  d30,d31,d32,d33:real;

implementation

{$R *.dfm}

procedure TForm1.Btn1Click(Sender: TObject);

begin
itera:=StrToInt(repet.Text);
while(repeticiones<itera)do
begin

if repeticiones=0 then
begin
//obtener valores
x01:=StrToFloat(x1.Text);
x02:=StrToFloat(x2.Text);
x03:=StrToFloat(x3.Text);
x04:=StrToFloat(x4.Text);
   //funciones
f1:=(pi*x01)-(e*x02)+(Sqrt(2*x03))-(Sqrt(3*x04))-(Sqrt(11));
f2:=(pi*pi*x01)+(e*x02)-(e*e*x03)+((3/7)*x04);
f3:=(Sqrt(5*x01))-(Sqrt(6*x04))+x03-(Sqrt(2*x04))-pi;
f4:=(pi*pi*pi*x01)+(e*e*x02)-(Sqrt(7*x03))+((1/9)*x04)-(Sqrt(2));



// aumenta el contador
repeticiones:=repeticiones+1;
end
else
begin

d00:=pi;
d01:=-e;
d02:=1/(Sqrt(2))*(Sqrt(x03));
d03:=-Sqrt(3)/(2*Sqrt(x04));

d10:=pi*pi;
d11:=e;
d12:=-e*e;
d13:=3/7;


d20:=Sqrt(5)/(2*Sqrt(x01));
d21:=-Sqrt(6)/(2*Sqrt(x02));
d22:=1;
d23:=-1/(Sqrt(2))*Sqrt(x04);

d30:=pi*pi*pi;
d31:=e*e;
d32:=-Sqrt(6)/(2*Sqrt(x03));
d33:=1/9;

//
d00:=1/d00;
d01:=1/d01;
d02:=1/d02;
d03:=1/d03;

d10:=1/d10;
d11:=1/d11;
d12:=1/d12;
d13:=1/d13;


d20:=1/d20;
d21:=1/d21;
d22:=1/d22;
d23:=1/d23;

d30:=1/d30;
d31:=1/d31;
d32:=1/d32;
d33:=1/d33;

//
f1:=-1*f1;
f2:=-1*f2;
f3:=-1*f3;
f4:=-1*f4;

//

h1:=f1*d00*d01*d02*d03*d10*d11*d12*d13*d20*d21*d22*d23*d30*d31*d32*d33;
h2:=f2*d00*d01*d02*d03*d10*d11*d12*d13*d20*d21*d22*d23*d30*d31*d32*d33;
h3:=f3*d00*d01*d02*d03*d10*d11*d12*d13*d20*d21*d22*d23*d30*d31*d32*d33;
h4:=f4*d00*d01*d02*d03*d10*d11*d12*d13*d20*d21*d22*d23*d30*d31*d32*d33;

x01:=x01+h1;
x02:=x02+h2;
x03:=x03+h3;
x04:=x04+h4;

//funciones
f1:=(pi*x01)-(e*x02)+(Sqrt(2*x03))-(Sqrt(3*x04))-(Sqrt(11));
f2:=(pi*pi*x01)+(e*x02)-(e*e*x03)+((3/7)*x04);
f3:=(Sqrt(5*x01))-(Sqrt(6*x04))+x03-(Sqrt(2*x04))-pi;
f4:=(pi*pi*pi*x01)+(e*e*x02)-(Sqrt(7*x03))+((1/9)*x04)-(Sqrt(2));



// aumenta el contador
repeticiones:=repeticiones+1;


end;// else
end;// end while

f04.Text:=FloatToStr(f4);
f03.Text:=FloatToStr(f3);
f02.Text:=FloatToStr(f2);
f01.Text:=FloatToStr(f1);


end;//boton

procedure TForm1.FormCreate(Sender: TObject);
begin
repeticiones:=0;
pi:=3.1415926535897932385;
e:=2.718281828459045235360;
end;

end.
