# FUPL
#FUPL interpretator 1.0.0.4
from random import*
from datetime import*
from sys import*
#from flask import*
import os

nom="FUPL"
stor="/storage/emulated/0"
stormyc=stor+"/1."+nom+"/"

if os.path.isdir(stormyc):
	pass
else:
	os.mkdir(stormyc)
# MYCRON GUI
imp=" import*\n"
frm="from "
t5yr=open(stormyc+nom+" GUI.py","w")
t='"\ "[0]+"t"'
t5yr.write(frm+"tkinter"+imp+
"from funksiya import* \n"+
"keng=5\n"+
"def tex(a,b):\n"+
"	w=Tk()\n"+
"	w.title(b)\n"+
"	f=Text(w, width=20, height=10)\n"+
"	f.grid()\n"+
"	f.insert(0.0,a)\n"+
"	w. mainloop()\n"+
"def oy():\n"+
"	w=Tk()\n"+
"	Button(text='<', command=exit, width=1).grid(row=1, column=2)\n"+
"	e1=Entry(width=18);e1.grid(row=1, column=1)\n"+
"	e2=Text(width=28, height=23);e2.grid(row=4, column=1) \n"+
"	def yoz():\n"+
"		a=str(e1.get())\n"+
"		import os\n"+
"		if os.path.exists(a):\n"+
"			e2.delete(0.0,END) \n"+
"			o=open(a,'r')\n"+
"			g=o.read()\n"+
"			o.close()\n"+
"			e2.insert(0.0,g)\n"+
"		else:\n"+
"			tex('File not found','ERROR')\n"+
"	def yozu():\n"+
"		e2.insert(END,'    ')\n"+
"	def ch():\n"+
"		z=str(e1.get())\n"+
"		v=str(e2.get(0.1,END)) \n"+
"		sfd=open(z,'w')\n"+
"		sfd.write('')\n"+
"		sfd.close()\n"+
"		g=open(z,'a')\n"+
"		g.write(v)\n"+
"		g.close()\n"+
"	def fl():\n\t\timport os\n\t\tc=str(e1.get())\n"+
"		if os.path.exists(c):\n"+
"			y=open(str(e1.get()),'w');y.write('');y.close()\n"+
"			tex('Cleared file','OK') \n"+
"		else:tex('File not found','ERROR')\n"+
"	def out(): \n"+
"		a=str(e2.get(0.0,END)) \n"+
"		exec(a) \n"+
"	Button(text='Read',command=yoz, width=keng).grid(row=2, column=1)\n"+
"	Button(text='Tab', command=yozu, width=keng).grid(row=2, column=1,sticky='nw')\n"+
"	Button(text='Save', command=ch, width=keng).grid(row=2, column=1,sticky='ne')\n"+
"	#Button(text='clear a file', command=fl).grid(row=6, column=2)\n"+
"	Button(text='>>', command=out, width=1, height=3).grid(row=4, column=2,sticky='n') \n"+
"	w. mainloop()\n"+
"oy()")
t5yr.close()
# MATEM
g67ytt=open(stormyc+"matem.py","w")
g67ytt.write('from math import*\n'+
'def ildiz(a):\n'+
'	return sqrt(float(a))\n'+
'def dar(a,b):\n'+
'	return float(a)**float(b)\n'+
'def discrim(a,b,c):\n'+
'     a=str(a);b=str(b);c=str(c)\n'+
'     a=QiymatXato(a); b=QiymatXato(b); c=QiymatXato(c)\n'+
'     d=b**2-4*a*c\n'+
'     if d<0:\n'+
'      print("-"),u()\n'+
'     if d==0:\n'+
'      print(-b/2*n),u()\n'+
'     if d>0:\n'+
'      d=sqrt(d)\n'+
'      x1=-b+d/2*a\n'+
'      x2=-b-d/2*a\n'+
'      print("x(v1)=%s"%x1,"x(v2)=%s"%x2)\n'+
'def taqqos(n,z):\n'+
'	if n==z:\n'+
'	    return str(n)+"="+str(z)\n'+
'	if n<z:\n'+
'	   return str(n)+"<"+str(z)\n'+
'	if n>z:\n'+
'		return str(n)+">"+str(z)\n'+
"def toq_juft(a):\n"+
"	if a%2==0:\n"+
"		return 'juft'\n"+
"	else:\n"+
"		return 'toq'\n"+
"def odd_even(a):\n"+
"	if toq_juft(a)=='juft': \n"+
"		return 'even' \n"+
"	else:\n"+
"		return 'odd' \n"+
"def katta(a,b):\n"+
"	return max(a,b)\n"+
"def kichik(a,b):\n"+
"	return min(a,b)\n"+
"def radi(a):\n"+
"	return radians(a)\n"+
"def grad(a):\n"+
"	return degrees(a)\n"+
"def yaxlit(a):\n"+
"	return round(a)\n"+
"def modul(a):\n"+
"	return abs(a)\n"+
"def ktyax(a):\n"+
"	return ceil(a)\n"+
"def kkyax(a):\n"+
"	return floor(a)\n"+
"def yaxn(a,b):\n"+
"	return round(a,b)\n"+
"" )
g67ytt.close()
# FIZIKA
g67ytt=open(stormyc+"fizika.py","w")
g67ytt.write(
frm+'math'+imp+
'g=9.81\n'+
"def physics_const():\n"+
"\tprint('g=9.81 N/kg')\n"
'def tezl_st(a,b):\n'+
'	return a/b\n'+
'def vaqt_sv(a,b):\n'+
'	return a/b\n'+
'def yOl_vt(a,b):\n'+
'	return a*b\n\n'+
'def kuch_mg(a):\n'+
'	return a*g\n'+
'def force_mg(a):\n'+
'	return a*g')
g67ytt.close()

# TURTLE
g67ytt=open(stormyc+"chizma.py","w")
g67ytt.write(
frm+"tkinter"+imp+
frm+"turtle"+imp+
"def o_ngchiz(a,b):\n"+
"	right(a)\n"+
"	forward(b)\n"+
"def chapchiz(a,b):\n"+
"	right(a); forward(b)" )
g67ytt.close()

mep="FEP"
hozir="04.03.22 20:38:12" #str(datetime.now())
versiya="1.0.0.5"
version=versiya
yang="("+hozir+")"
ekr=nom+" ["+versiya+"] android uchun.\n"+yang+"\nKoʻproq maʼlumot 'mualliflik', 'yordam' yoki  'tarix' soʻzlarida."
screen=nom+" ["+versiya+"] for android.\n"+yang+"\nType 'help', 'copyright' or 'history' for more information."

tas=randint(1,2)
if tas==1:# oʻzbek
  print(ekr)
if tas==2:# ingliz
  print(screen)
 
def FaylMavjudEmasligiXato(b):
	return "X 1==\nFl-X:","'"+b+"' Fl- "

def FaylMavjudligiXato(b):
	return "X 1==\nFl+X: + '"+b+"' Fl"

def ModulMavjudEmasligiXato(b):
	return "X 1==\nM-X: M '"+b+"' -"

def NomXato(b):
	return "X 1==\nNX: N '"+b+"'-"

def QiymatXato(b):
	return "X: 1 ==\nQX: '"+b+"' ~No"

def SintaksisXato(c,b):
  if b not in c :
   print("X:",1,"==\nSX: v'"+b+"' "),u()
def SintaksisXato(b):
 return "X: 1==\nSX:\n\t"+b
 
def Xato(a):
	try:
		a+"g"
	except TypeError:
		QiymatXato(str(a))
	except ValueError:
		QiymatXato(str(a))
	except NameError:
		NomXato(str(a))
	except SyntaxError:
		SintaksisXato(a)

# BOSHQA
def output(a):
	a=str(a)
	f=open(a,"r")
	n=f.read()
	f.close()
	try:
		print(n,"\n")
		exec(n)
		return ''
	except SyntaxError:
		return "SX:\n"+n
	except NameError:
		return "NX: N '"+a+"' -"
def natija(a):
	return output(str(a))

def file(a):# YOZISH
  	f=str(a)
  	s=0
  	open(f,"w"). close()
  	while True:
  		r=open(f,"a")
  		s+=1
  		d=input(str(s)+"__|")
  		if "save"in d or "saqla"in d :
  			return output(f)
  		else:
  			"save" not in d and "saqla"not in d
  			r.write(d+"\n");r.close()

# FAYLLAR
def qo_sh(a,b):
	a=str(a);b=str(b)
	j=open(a,"a")
	j.write(b)
	o=j.close()
	return ''
def appen(a):
	a=str(a)
	qo_sh(a)

def o_chir(a):
	a=str(a)
	import os
	try:
		os.remove(a)
		return ''
	except FileNotFoundError:
		return FaylMavjudEmasligiXato(a)
def remove(a):
	a=str(a)
	o_chir(a)
	return ''

def yozish(a,b):
	a=str(a);b=str(b)
	t=open(a,'w')
	t.write(b)
	g=t.close()
	return ''
def write(a,b):
	a=str(a);b=str(b)
	yozish(a,b)
	return ''

def qaytnomfl(a,b):
	a=str(a);b=str(b)
	import os
	if os.path.exists(a):
		if os.path.exists(b):
			FaylMavjudligiXato(b)
		else:
			os.rename(a,b)
			return ''
	else:
		FaylMavjudEmasligiXato(a)
def rename(a,b):
	a=str(a);b=str(b)
	qaytnomfl(a,b)
	return ''

def yrtfl(a):
	a=str(a)
	import os
	if os.path.exists(a):
		FaylMavjudligiXato(a)
	else:
		open(a,"x")
		return ''
def mkfl(a):
	a=str(a)
	yrtfl(a)

def o_qish(a):
	a=str(a)
	t=open(a,"r")
	f=t.read()
	t.close()
	return f
def read(a):
	a=str(a)
	return o_qish(a)

def aniq(a):
	a=str(a)
	import os
	if os.path.exists(a):
		return True
	else:
		return False
def todtrfl(a):
	return aniq(a)

def ktyar(a):
	os.mkdir (str(a))
	return ''
# SOʻZLAR
def mirror(a):
	a=str(a)
	return a[::-1]
def aks(a):
	a=str(a)
	return a[::-1]

def uzun(a):
	a=str(a)
	return len(a)

def da(a,b):
	a=str(a);b=str(b)
	if b in a:
		return True
	if b not in a:
		return False
def in_(a,b):
	a=str(a);b=str(b)
	if a in b:
		return True
	if a not in b:
		return False

def tur(a):
	return type(a)

def kirit(*a):
	return input(a)

def pas():
	None

# CASElar
def if_t_t(a,b):
	if a==b:
		return True
	else:
		return False

# VAQT, SOAT
def hozir():
	return datetime.now()
def now():
	return hozir()

def pas():
	pass

# STANDART OPERATORLAR
def yozuv(*a):
	return print(str(a)[1:-1])

def kirit(*a):
	return input(str(a)[1:-1])

def pas():
	pass
def yordam():
       buy=">>> "
       iz="  # "
       f=open(stormyc+nom+" qoʻllanma.txt","w")
       f.write('\t\tFUPL QOʻLLANMASI'+
       "\n\t\tBAʼZI ATAMALAR\n"+
       "Argument- funksiya qabul qiladigan qiymatlarning belgilangan soni\n"+
       "Operator- dasturlash tili buyrugʻi\n"+
       "Modul- alohida faylda yozilgan funksiyalar majmuasi."+
       "\tFUPL TARIXI\n"+
       '  '+nom+' (The first uzbek programming language - Birinchi oʻzbekcha dasturlash tili) dasturlash tilining muallifi — QUCHQOROV Kamronbek.Ushbu qoʻllanma '+nom+'ni oʻrganish uchun yaratildi. Qoʻllanma '+nom+'ning '+versiya+' versiyasi boʻyicha yaratildi. Endi esa '+nom+' tarixiga yuzlansak: dasturlash tiliga dastlab "Mycron" deb nom qoʻyilgan edi. Ammo keyinchalik "'+nom+'"ga aylandi.\n'+
       "  "+nom+" dasturlash tilining quyidagicha qulayliklari bor:\n"+
       "1)Oʻzbek va ingliz tillarida ishlay olishi;\n"+
       "2) Sodda sintaksisga ega eksnligi;\n"+
       "3)Unda python dasturlash tilining kodlarini yozish va undan foydalanish imkonining mavjudligi;\n"+
       "4) Dastur oʻz matn muharririga ega."
       '  Dasturlash tilining eng ajoyib jihati shundaki, u ham ingliz, ham oʻzbek tilida ishlay oladi. Shu sababli buyruqlar ham ikki xil.Biz bu ikki kalit soʻzlarni "/" belgisi yordamida ajratdik.\n'+
       '\t'+nom+' INTERFEYSI VA KICHIK BUYRUQLAR\n'+
       ' Ushbu dasturlash tilining interfeysi har doim har xil koʻrinishga ega boʻladi. Bu mutlaqo tasodifiy tarzda roʻy beradi:\n'+
       ekr+'\n'+buy+'#1\n'+
       screen+'\n'+buy+'#2\n'+
       "  '"+buy+"' belgisidan keyin buyruq kiritish mumkin. Quyida misol:\n"+
       buy+"yozuv('Salom dunyo!')\n"+
       "Salom dunyo!\n"+
       "\t"+nom+"da DASTUR TUZISH\n"+
       "  "+nom+"da dastur tuzish uchun (boshqa dasturlash tillari kabi) operatorlarni maʼlum tartibda joylashtirish kerak. Hozir biz 'yozuv' va 'kirit' operatorlarlari bilan tanishamiz.\n"+
       "  Bu funksiyalarning vazifasi bir xil, ammo ular turlicha argument qabul qiladi. Argumentlar orasida nechta vergul boʻlsa, shu sondan bitta koʻp argument kiritilgan boʻladi.\n"+
       "  yozuv operatorlar oilasi kiritilgan soʻzni ekranga chiqarish vazifasini bajaradi. kirit operatorlar oilasi esa qavs ichida yozilgan soʻzni ekranga chiqarib, qiymat kiritishni soʻraydi. Quyida misol:\n"+
       buy+"kirit(\"Soʻz: \")\n"+
       "Soʻz: (Shu yerga soʻz yozing)\n"+
       "(Shu yerga soʻz yozing)\n"+
       "  "+nom+"da fayllarni ishgs tushirish mumkin. Buning uchun file() operatori qoʻl keladi. Funksiya bitta argument qabul qiladi va shu nomdagi faylga endi kiritadigan yozuvlarni yozadi. Agar fayl mavjud boʻlmasa, yaratadi va yozadi. Agar mavjud boʻlsa, ichidagi barcha yozuvlar oʻchib, yangi yozuvlar yoziladi.Barcha yozuvlar saqlanib, dastur ishga tushishi uchun \"save\" yoki \"saqla\" soʻzlaridan birini kiritish kerak. Shunda fayl saqlanadi va dasturimiz ishga tushadi. Quyida misol:\n"+
       buy+"file('salom')\n"+
       "1__|yozuv(\"Salom dunyo!\")\n"+
       "2__|save\n\n"+
       "Salom dunyo!\n"+
       "  Agar fayl mavjud boʻlsa va unda "+nom+"ga doir yozuvlar boʻlsa, faylni natija() yoki output() funksiyalari orqali ishga tushirish mumkin. Quyida misol:\n"+
       buy+"output('salom')\n"+
       "yozuv(\"Salom,\",\"doʻstim\")\n\n"+
       "Salom, doʻstim\n"+
       '\t'+nom+'DA IZOHLAR BILAN ISHLASH\n'+
       ' '+nom+' dasturlash tilida izoh yozish pythonnikiga oʻxshab ketadi. Masalan, 1 satrli izoh yozish uchun "#" belgisidan foydalaniladi. Buning uchun '+buy+' belgisidan keyin "#" beligisi kiritiladi. Soʻng izoh yozish mumkin.Quyida misol keltirilgan:\n\n'+
        ' '+buy+' #Salom. Yaxshimisiz?\n'+' '+buy+'\n\n'+
        'Endi esa koʻp qatorli izohlar bilan ishlashni oʻrganamiz. Buning uchun satr boshiga 3 ta (bittalik yoki ikkitalik qoʻshtirnoq qoʻyish kerak. Keyin esa izohni yakunlash uchun yana ikkitalik yoki bittalik qoʻshtirnoq qoʻyish kerak. Quyida misol keltirilgan:\n\n'+
        buy+'"""Salom. Ahvolim juda yaxshi\n'+
        iz+'Qoyil\n'+
        iz+'Tamom""" \n'+
        buy+'\n\n'+
        "\tOʻZGARUVCHILAR BILAN ISHLASH\n"+
        '\tSOʻZLAR BILAN ISHLASH\n'+
        ' '+nom+'da ham soʻzlar ustida ishlash mumkin. Buning uchun 3 ta buyruq mavjud. Ular quyidagilar:\n'+
        '  aks/mirror--------------soʻzni akslantiradi\n'+
        '  in_/da------------------------a b ning ichidaligini aniqlash\n'+
        '  uzun/len------------------soʻz uzunligini aniqlash\n'+
        'Bu buyruqlar dasturda quyidagicha ishlatiladi:\n\n'+
        buy+'  in_("f","uj")\n'+
        '  0\n'+
        buy+'  da("gol","g")\n'+
        '  1\n'+
        buy+'  len("salom!")\n'+
        '  6\n'+
        buy+'  uzun("bolakay")\n'+
        '  7\n'+
        buy+'  aks("salom")\n'+
        '  molas\n'+
        buy+'  mirror("salom")\n'+
        '  molas\n\n'+
        "\t MODULLAR \n"+
        "  Modullar foydalanish uchun juda qulay. "+nom+"da quyidagi modullar mavjud:\n"+
        "1) fizika- ushbu modul fizikaga oid maʼlumotlarni berish va masalalarni hal etish imkonini beradi;\n"+
        "2)chizma- modul turli chiziq va figuralarni chizish uchun ishlatiladi;\n"+
        "3)matem- Matematik, trigonometrik hisoblashlarni amalga oshiruvchi modul;\n"+
        '\tMATEMATIK HISOBLASH\n'+
        '  '+nom+' dasturlash tilida ham matematik funksiyalar mavjud. Ularning barchasi matem moduliga joylashtirilgan. Avval bu modulni dasturga yuklash kerak . Ulardan foydalanish uchun quyida misollar keltirilgan:\n\n'+
        '   '+buy+'sin(34)\n'+
        '   529082686120\n\n'+
        ' Bundan tashqari boshqa buyruqlar quyida keltirilgan:\n'+
        ' sin--------------------sinus\n'+
        ' cos-------------- kosinus\n'+
        ' tan---------------tangens\n'+
        ' atan-------arktangens\n\n'+
        ' log10-------------------oʻnli logarifm\n\n'+
        ' toq_juft/odd_even-----toq yoki juft\n'+
        ' taqqos------------------------taqqoslash\n'+
        ' katta/max------------------eng katta son\n'+
        ' kichik/min------------------eng kichik son\n'+
        ' radi----------------------------darajadan radianga\n'+
        ' grad----------------------------radiandan darajaga\n'+
        ' kkyax--------------------------eng yaqin kichik butun songacha yaxlitlash\n'+
        ' yaxlit--------------------------yaxlitlash\n'+
        ' yaxn(m,n)-----------------yaxlitlash (m ni n ta belgi qolguncha yaxlitlash)\n'+
        ' ktyax--------------------------eng yaqin katta butun songacha yaxlitlash\n'+
        ' factor------------------------faktorial\n'+
        ' pi------------------------------pi soni\n'+
        ' ild----------------------kvadrat ildiz\n'+
        ' modul------------------modul\n'+
        ' log--------------------------------logarifm(a,b)\n'+
        ' discrim-----------------------(a,b,c)diskriminant\n'+
        ' modul(a)------------a ning moduli\n'+
        '\tFIZIKA\n'+
        ' '+nom+' dasturlash tilida fizik masalalarni ham hisoblash mumkin.\n'+
        ' kuch_mg(a)-----------------a ning ogʻirlik kuchini hisoblaydi (g=9.81 N/kg)\n'+
        ' fizik_const/physics_const------------fizik konstantalarni chiqaradi\n'+
        ' tezl_st(a,b)----------------a/b tezlikni hisoblaydi\n'+
        ' yo_l_vt(a,b)---------------a*b masofani hisoblaydi\n'+
        ' vaqt_sv(a,b)-------------a*b masofa\n'+
        '\tXATOLAR BILAN ISHLASH\n'+
        '  Agar dasturga dasturdagi kalit soʻzlardan boshqa soʻz kiritilsa, quyidagi xatolik ekranga chiqadi.\n\n'+
        buy+'hhh\n'+
        'X:  1 ==\n'+
        'NX: N "hhh"\n'+
        buy+'\n\n'+
        ' Xatolar bilan ishlash uchun baʼzi belgilarning bildiradigan soʻzlarini bilib olish zarur:\n'+
        ' "Fl"-------"Fayl"\n'+
        ' "X"-----"xato"\n'+
        ' "N"-----"nom"\n'+
        ' "+"------"allaqachon mavjud"\n'+
        ' "-"--------"mavjud emas"\n'+
        ' "Q"------"qiymat"\n'+
        ' "S"-------"Sintaksis"\n'+
        " '~'------'emas' \n"+
        " '_'-------'kiritish' \n"+
        " 'kk'-----'kichik' \n"+
        " 'kt'------'katta' \n"+
        '  NomXato(NX), FaylMavjudligiXato(Fl+X), FaylMavjudEmasligiXato(Fl-X), QiymatXato(QX),SintaksisXato(SX) bular xatolik turlari hisoblanadi. Xatoga yoʻl qoʻyishning quyidagi sabablari boʻlishi mumkin: verguldan soʻng boʻsh joy qoldirish, ikkita vergulni yonma-yon qoʻyish va raqam oʻrniga soʻz yoki belgi kiritish.\n'+
        '\tFAYLLAR BILAN ISHLASH\n'+
        " Quyida fayllar bilan bogʻliq funksiyalar.\n "+
        ' yrtfl/mkfl-------------------Fayl yaratadi\n'+
        ' o_chir/remove-----------------------Faylni oʻchiradi\n'+
        ' o_qish/read--------------------------------Faylni oʻqiydi\n'+
        ' qo_sh/appen-----------Faylga yozuv qoʻshadi(Agar mavjud boʻlmasa, yaratib yozadi)\n'+
        ' yozish/write--------------Faylga qayta yozadi(barcha eski yozuvlar oʻchib, yangisi yoziladi. Agar fayl mavjud boʻlmasa yaratib yozadi)\n'+
        ' qaytnomfl/rename-------Faylni qayta nomlaydi(mavjud boʻlmasa xatolik yuz beradi)\n\n'+
         'aniqfl/todtrfl-------------------Fayl mavjudligini aniqlaydi(mavjud boʻlsa 1, aks holda 0 ni qaytaradi)'+
         "ktyar------------------- katalog yaratish\n" )
       f.close()
       print("\n\t"+nom+" "+versiya+" yordam dasturiga xush kelibsiz!\nAgar "+nom+"dan birinchi marta foydalanayotgan bo'lsangiz, albatta tekshirib ko'rishingiz kerak.\nYozish bo'yicha yordam olish uchun har qanday modul, kalit so'z yoki mavzu nomini kiriting.\n\t"+nom+" dasturlari va "+nom+"  modullaridan foydalanish.\nUshbu yordam dasturidan chiqish va tarjimonga qaytish uchun, shunchaki, \"chiqish\" ni kiriting.\nMavjud modullar, kalit so'zlar yoki belgilar  ro'yxatini olish uchun\n\"modullar\", \"belgilar\", 'hujjat'  yoki 'FEP' soʻzlaridan birini kiriting.\n")
       while True:
       	pr=input("yordam > ")
       	if "modullar"in pr:
       		print("Modullar roʻyxati:\n\tchizma\n\tmatem\n\tfizika")
       	if "chiqish"in pr:
       		return ''
       		break
       	if "FEP"in pr or "fep"in pr :
       		print("  Qurilmangizning '.FUPL' katalogida\n'"+mep+".txt' nomli fayl paydo boʻldi.\nIltomos, qurilmangizni tekshiring!")
       		f=open(stormyc+mep+".txt","w")
       		f.write("\tAgar siz oʻzbek tilini bilsangiz "+mep+" hujjatlari quyidagicha yoziladi:\nYaratdi: (ism, familiya)\nBoshlandi: (yaratish boshlangan vaqt(sana,oy,yil))\nTugatildi: (yaratish tugallangan vaqt(sana,oy,yil))\nVersiya:(Qaysi versiya boʻyicha yaratilgani.)\nMen quyidagilarni taklif qilmoqchiman:\n1)______(1-taklif);\n2)_____(2-taklif)\n...\n\t(Agar savollar boʻlsa, quyidagicha:)\nQuyidagi savollarim bor:\n1)____(1-savol)\n2)____(2-savol)\n...\n\n\tDIQQAT!\nQachon "+mep+" soxta deb topiladi?\nQachonki, hujjatda:\n1.Bezakdor, badiiy, erkalash soʻzlari boʻlsa;\n2.Baʼzi parametrlar koʻrsatilmasa;\n3.Fayl py, my, txt kabi fayllardan birortasiga ham tegishli boʻlmasa;\n4."+mep+" muddati oʻtgan boʻlsa.\n\tESDA SAQLANG!\n"+mep+" yozishda fayl nomi '"+mep+'+('+mep+" raqami).txt' koʻrinishida belgilanishi kerak.\n\nYaratilayotgan fayl txt, my yoki py koʻrinishida boʻlishi mumkin."+mep+"larni fupl.uz@mail.ru elektron pochta manziliga yuborishingiz mumkin!")
       		f.close()
       	if "belgilar"in pr:
       		print("%\t|\t==\t<\n>\t^\t&\t-\n+\t/\t//\t*\n**\t>>\t<<")
       	if "hujjat"in pr:
       		print(o_qish(stormyc+nom+" qoʻllanma.txt"))
def help():
	pass

def mualliflik() :
	return "Mualliflik huquqi (c) 2022.\nBarcha huquqlar himoyalangan."
def copyright() :
	return "Copyright (c) 2022\nAll Rights Reserved."

def tarix() :
    return nom+" dasturlash tilining muallifi- Kamronbek QUCHQOROV.\n Dasturni yaratish 2021-yilda boshlangan.\n"
    return ''
def license() :
    print("License: MIT")

def stop():
	while True:
		buy=">>> "
		iz="  # "
		m=input(buy)
		if "#"in m:
				if m[0]=="#":
					u()
		if m[:3]=="\'\'\'":
				while True:
					i=input(iz)
					if i[:-4:-1]=="\'\'\'":
						u()
					else:
						pass
		if m[:3]=="\"\"\"":
				while True:
					i=input(iz)
					if i[:-4:-1]=="\"\"\"":
						u()
					else:
						pass
		if m.lstrip()=='' or m=='' :
			pass
		else:
			a=m
			if ("="in a and "=="not in a)or("import"in a)or("def"in a)or("while"in a) :
				exec(a)
			else:
				"print"not in a and "yozuv"not in a
				try:
					print(eval(a))
				except SyntaxError:
					print (SintaksisXato(a))
				except NameError:
					print(NomXato(a))
				except TypeError :
					print()
				except ValueError:
					print()
				except AttributeError:
					print()
				except EOFError:
					print()
				except OSError:
					print()
				except IsADirectoryError:
					print()
stop()

"""
app = Flask(__name__)
@app.route("/")
def hello():
  return "3.Mycron/Mycron.py"
if __name__ == "__main__":
  app.run()"""
