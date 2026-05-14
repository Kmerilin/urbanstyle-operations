WEEK 2: Tiimi koondraport 

1. Mis oli suurim üllatus?

Suurimaks üllatuseks oli väga suur duplikaatide hulk mitmes tabelis. Eriti paistsid silma:
	•	4013 duplikaati veerus ja 5116 duplikaatset müügirida müügiandmetes
	•	380 duplikaatset e-maili kliendiandmetes
	•	592 klienti, kes pole kunagi midagi ostnud
Samal ajal oli positiivne üllatus, et tooteandmetes olid kõik kriitilised väljad olemas ning puudusid erinevad nimekujud nagu “Shoes” vs “shoes”.
Kõige kehvemas seisus olid kliendi- ja müügiandmed.
Tooteandmed olid võrreldes teiste domeenidega kõige puhtamad. 

2. Milline on meie soovitus Toomasele?

Peamine soovitus on:
	1	eemaldada duplikaadid,
	2	korrastada kliendiandmed,
	3	valideerida hinnad ja seosed tabelite vahel

Andmeid saab pärast puhastamist rohkem usaldada, kuid täielikku usaldusväärsust veel ei ole saavutatud.
Edasine prioriteet võiks olla:
	1	eemaldada duplikaadid,
	2	parandada NULL-väärtused ja puuduvad kontaktid,
	3	kontrollida hinnaloogikat,
	4	eemaldada vaimkliendid ja vaimtooted,
	5	luua automaatsed valideerimisreeglid.

Kõige kriitilisemad probleemid on need, mis mõjutavad äriotsuseid ja kliendisuhtlust.

3.Milliseid andmeid meil puudus?

Puudusid:
	•	kliendi kontaktandmed (380 NULL e-maili),
	•	customer_id väärtused müügiandmetes,
	•	usaldusväärne info mõne müügihinna kohta, sest 20 toote hinnad ei klappinud toote hinnakirjaga.

4. Kas oli olukordi, kus me ei teadnud, mis on “õige” väärtus?
	•	kui kliendi e-mail oli NULL, ei olnud võimalik teada, milline kontaktinfo on õige;
	•	duplikaatsete e-mailide puhul ei olnud alati selge, milline kliendikirje oli korrektne;
	•	hinnavastuolude korral ei olnud võimalik kindlalt öelda, kas vale oli müügihind või toote baasandmed;
	•	“vaimklientide” puhul ei olnud teada, kas tegemist oli vigase impordi, vanade klientide või testandmetega
