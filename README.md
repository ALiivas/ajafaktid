# ajafaktid
Korpus loodi Annely-Maria Liivase bakalaureusetöö *Ajaväljendite korpusemärgenduse laiendamine sündmuste ja entiteetide ajalisteks omadusteks TimeML raamistikus* raames. Korpusetekstid pärinevad eesti keele ajaväljendite korpusest (EstTimexCorpora). Olemasolevale ajaväljendite märgendusele lisati bakalaureusetöö raames ajaväljenditega seotud sündmuste ja entiteetide märgendus.

Kaust *korpus_brat* sisaldab korpuse BRAT-i versiooni ehk *.ann* ja *.txt* faile ning konfiguratsioonifaili *annotation.conf*.

Kaust *korpus_json* sisaldab korpuse EstNLTK json kujul versiooni.

Korpuse teisendamisel BRAT-i kujult EstNLTK json kujule kasutati skripti *convert_BRAT_to_estnltk_json.py* (kättesaadav aadressil https://github.com/soras/EstTimexCorpora/blob/master/scripts/convert_BRAT_to_estnltk_json.py).

Eelnõuded: `Python 3.7+` `EstNLTK 1.6.9+`

Json kujul versiooni kasutamisel tuleb Pythonis kaust sisse lugeda. Dokumendid salvestatakse EstNLTK *Text* objektidena.

*Text* objektidel on järgnevad märgenduskihid:

`brat_entities` - abikiht mitmesõnaliste ja katkendlike märgenduste jaoks

`entities` - entiteedid

`events` - sündmused

`timexes` - ajaväljendid

`tlinks` - ajaseosed

`has_argument` - argumentseosed sündmuste vahel
