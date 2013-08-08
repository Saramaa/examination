Ramverket Lycka
=====

Lycka är ett MVC (Model view controller) skapat av Anderz Johansson.

Installation
============

<h4>1. Ladda ner ramverket Lycka till din dator</h4> 
Det första steget du måste göra är att klona ramverkets kod. Detta gör du via programmet 
GitBash(http://git-scm.com/downloads). När du är redo att klona koden till aktuell katalog skriver du in: <code>git clone https://github.com/Saramaa/examination.git</code>.
Du kan även gå till sidan https://github.com/Saramaa/examination och klicka på ikonen "Download ZIP" för att få projektet i ZIPformat.

<h4>2. Ladda upp ramverket på en webserver och gör site/data skrivbar</h4> 
När du har koden på din dator är det dag att skicka koden till en webserver. 
Detta gör du förslagsvis med FilZilla(https://filezilla-project.org/). Det första du bör gör är att göra mappen kmom8/site/data skrivbar. Detta kan du göra via FileZilla(högerklicka på
mappen site/data. Välj sedan "Filrättigheter". Fyll i "777" i det numeriska värde fältet. Kryssa sedan i "Upprepa i underkataloger" samt "Verkställ på alla filer och kataloger". Klicka sedan på "OK"
och du är klar).

<h4>3. Konfigurera filen .htacces</h4>
I mappen "kmom8" finn filen ".htacces". Öppna denna fil och du ser kodraden <code>RewriteBase /~anjo13/phpmvc/kmom7/</code> på rad 2. Denna kod
skall du ändra så att det stämmer överens med din användare(om du te.x använder BTH's webserver).

<h4>4. Installera moduler</h4> När du sedan går in på ramverket kommer du till sidan "Index Controller". Under rubriken "Installation" skall du klicka på
knappen "module/install". När detta är gjort möts du av ett meddelande som verifierar att initialiseringen är klar. Det skapas två
användare med namn/lösenord "doe/doe" och "root/root". Nu är installationen klar! 



Utföra egna ändringar i Lycka
===============================

För att utföra egna ändringar i Lycka skall du gå till filen config.php som du finner i katalogen kmom8/site/.
Här finns det flertalet saker du kan ändra:
<h4>Logo</h4>
Om du vill ändra logo så lägger du till din nya logo i site/themes/myThemes mappen. Sedan ändrar du kodraden <code>'logo' => 'lycka.jpg'</code>
i config.php till namnet på din egen bild.
<h4>Titel</h4>
För att ändra namnet på titeln går du till kodraden <code>'header' => 'Lycka'</code> och tar bort "Lycka" och ändrar
till den titeln du vill ha.
<h4>Footer</h4>
För att byta footer går du till kodraden  <code>'footer' => '<p>Lycka &copy; by Anderz Johansson</p>'</code> och ändrar innehållet
till något valfritt.
<h4>Navigation</h4>
I "'my-navbar' => array(" arrayen kan du ändra navigeringsmenyn. Om du tex vill byta namnet på "My Blog" går du till kodraden
<code>'blog'      => array('label'=>'My Blog', 'url'=>'my/blog')</code> och ändrar <code>'My Blog'</code> till vad du önskar.

Ändra tema
===========
Öppna filen <code>kmom8/site/themes/mythemes/style.css</code>. Detta är CSS-filen för ramverkets tema.

Skapa innehåll
==============
Anvisningar för att skapa innehåll för blog och sida:
<h4>Blog</h4>
(1)Klicka på "My blog" i menyn. (2)Klicka på "edit" på ett av de bloginlägg som har lagts in som default. (3) Klicka på "Create new".
(4) Fyll i de olika fälten. Tänk på att type skall vara "post" och Filter skall vara "plain".
<h4>Sida</h4>
(1) Klicka på "About Me" i menyn. (2) Klicka på "edit". (3) Klicka på "Create new". (4) Fyll i fälten. Tänk på att type skall vara "post" och Filter skall vara "plain".
