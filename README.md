learnGitHub
===========

Instruktioner f�r att snabbt och enkelt komma ig�ng med github.

0: Skapa anv�ndare p� github.com
1: Ladda ner Git fr�n http://git-scm.com/
2: F�lj instruktionerna och v�lj "Run Git from the Windows Command Promt" och "Checkout Windows-Style" alternativen n�r tillfr�gad.
3: git config --global user.name "AntonAderum"
4: git config --global user.email antonaderum@gmail.com
5: cd ~/.ssh
6: mkdir key_backup
   cp id_rsa* key_backup
   rm id_rsa*
(om det redan fanns en ssh-nyckel)
7: ssh-keygen -t rsa -C "your_email@example.com" 
8: Det kommer komma lite fr�gor om vart man vill lagra nyckel och om passphrases, det g�r bra att bara trycka enter + enter + enter.
9: clip < ~/ssh/id_rsa.pub
10: Account Settings -> SSH Keys -> Add SSH key -> * klistra in nyckeln i textf�ltet * - > Add Key -> Fyll i Github l�senord
11: ssh -T git@github.com
12: Ovanst�ende f�rs�ker g�ra en anslutning till github, kommandotolken kommer att fr�ga om du vill autentisera github.com, skriv "yes" och g� vidare.
13: Om "Hi xxxx! .." kommer upp s� har allting lyckats.
14: G� till https://github.com/AntonAderum/learnGitHub i webbl�saren och tryck p� "Fork" knappen. Detta kopierar hela mitt projekt till eran Github anv�ndare.
15: Anv�nd kommandotolken och g� till mappen d�r du vill ladda ner projektet.
16: git clone git@github.com:XXX/learnGitHub.git
17: �ndra i iWasHere.txt och fyll i ditt namn. ANv�nd valfri editor
18: git status
19: git add - A
20: git commit - "Jag skrev in mitt namn"
21: git status
22: G� till erat github-projekt och tryck p� "Pull Request" och f�lj instruktionerna
23: Klart!

Andra andv�ndbara commandon.
git pull : h�mtar den mest uppdaterade versionen av githubprojektet som du st�r i. 
