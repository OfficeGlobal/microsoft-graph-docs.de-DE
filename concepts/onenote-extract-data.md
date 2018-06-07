# <a name="use-onenote-api-div-tags-to-extract-data-from-captures"></a>Verwenden von div-Tags der OneNote-API zum Extrahieren von Daten aus Erfassungen 

*__Gilt für:__ Privatanwender-Notizbücher auf OneDrive | Enterprise-Notizbücher auf Office 365*

Verwenden Sie die OneNote-API zum Extrahieren von Visitenkartendaten aus einem Bild oder von Rezept- und Produktdaten von einer URL.

<a name="attributes"></a>
## <a name="extraction-attributes"></a>Extraktionsattribute

Zum Extrahieren und Transformieren von Daten schließen Sie einfach ein div-Tag in die [create-page](onenote-create-page.md)- oder [update-page](onenote_update_page.md)-Anforderung ein, das den Quellinhalt, die Extraktionsmethode sowie ein Ausweichverhalten angibt. Die API rendert extrahierte Daten auf der Seite in einem einfach zu lesenden Format. 

```
<div
  data-render-src="image-or-url"
  data-render-method="extraction-method"
  data-render-fallback="fallback-action">
</div>
```

**data-render-src**

Die Inhaltsquelle. Dies kann ein Bild einer Visitenkarte oder eine absolute URL von zahlreichen beliebten Rezept- oder Produktwebsites sein. Erforderlich. 

Verwenden Sie für optimale Ergebnisse beim Angeben einer URL die kanonische URL, die ggf. im HTML-Code der Quellwebseite definiert ist. Eine kanonische URL kann beispielsweise folgendermaßen in der Quellwebseite definiert werden:

`<link rel="canonical" href="www.domainname.com/page/123/size12/type987" />` 


**data-render-method**

Die auszuführende Extraktionsmethode. Erforderlich. 

| Wert | Beschreibung |
|:------|:------|
| extract.businesscard | Extraktionen von Visitenkarten. |
| extract.recipe | Extraktionen von Rezepten. |
| extract.product | Extraktionen von Produktlisten. |
| extract | Ein unbekannter Datenextraktionstyp. |

Für optimale Ergebnisse geben Sie den Inhaltstyp (`extract.businesscard`, `extract.recipe` oder `extract.product`) an, falls bekannt. Wenn der Typ nicht bekannt ist, verwenden Sie die `extract`-Methode; die OneNote-API versucht daraufhin, den Typ automatisch zu ermitteln.

**data-render-fallback**

Das Ausweichverhalten, wenn die Extraktion fehlschlägt. Wenn der Wert weggelassen wird, gilt der Standardwert **render**. 

| Wert | Beschreibung |
|:------|:------|
| render() | Rendert das Quellbild oder eine Momentaufnahme der Rezept- oder Produktwebseite. |
| n/v | Hat keine Wirkung. <br />Die Option ist nützlich, wenn Sie zusätzlich zum extrahierten Inhalt immer eine Momentaufnahme der Visitenkarte oder Webseite auf der Seite einschließen möchten. Achten Sie darauf, ein separates `img`-Element in der Anforderung zu senden, wie in den Beispielen dargestellt. |

<a name="biz-card"></a>
## <a name="business-card-extractions"></a>Extraktionen von Visitenkarten

Die OneNote-API sucht und rendert die folgenden Kontaktinformationen basierend auf dem Bild einer Visitenkarte einer Person oder eines Unternehmens.


- Name
- Titel
- Organisation
- Telefon- und Faxnummer
- Postanschrift und physische Adressen
- E-Mail-Adressen
- Websites
   
  ![Ein Beispiel für die Extraktion einer Visitenkarte.](images/biz-card-extraction.png)

Eine vCard (VCF-Datei) mit den extrahierten Kontaktdaten wird auch in die Seite eingebettet. Die vCard ist eine bequeme Möglichkeit, um die Kontaktinformationen beim Abrufen des HTML-Inhalts der Seite abzurufen.

### <a name="common-scenarios-for-business-card-extractions"></a>Häufige Szenarien für Visitenkartenextraktionen

**Abbildung zum Extrahieren von Visitenkarteninformationen und Rendern der Visitenkarte**

Geben Sie die `extract.businesscard`-Methode und das `none`-Ausweichverhalten an. Senden Sie auch ein `img`-Element mit dem `src`-Attribut, das auch auf das Bild verweist. Wenn die API keinen Inhalt extrahieren kann, wird nur das Bild der Visitenkarte gerendert.

```html 
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard"
    data-render-fallback="none">
</div>
<img src="name:scanned-card-image" />
```


**Abbildung zum Extrahieren von Visitenkarteninformationen und Rendern des Bilds der Visitenkarte, wenn die Extraktion fehlschlägt**

Geben Sie die `extract.businesscard`-Methode an, und verwenden Sie das standardmäßige `render`-Ausweichverhalten. Wenn die API keinen Inhalt extrahieren kann, wird stattdessen das Bild der Visitenkarte gerendert.

```html
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard">
</div>
```
 
Bei Visitenkartenextraktionen wird das Bild als benannten Teil in einer mehrteiligen Anforderung gesendet. Unter [Hinzufügen von Bildern und Dateien](onenote_images_files.md) finden Sie Beispiele, in denen gezeigt wird, wie ein Bild in einer Anforderung gesendet wird.


<a name="recipe"></a>
## <a name="recipe-extractions"></a>Extraktionen von Rezepten

Die OneNote-API sucht und rendert die folgenden Informationen auf der Grundlage einer Rezeptkarten-URL.

- Großformatiges Hintergrundbild
- Bewertung
- Zutaten
- Anweisungen
- Vorbereitungs-, Koch- und Gesamtzeiten
- Portionen

   ![Ein Beispiel für die Extraktion von Rezepten](images/recipe-extraction.png)

Die API ist für Rezepte von vielen beliebten Websites wie *Allrecipes.com*, *FoodNetwork.com* und *SeriousEats.com* optimiert.

### <a name="common-scenarios-for-recipe-extractions"></a>Häufige Szenarien für Rezeptextraktionen

**Extrahieren von Rezeptinformationen und Rendern eines Snapshots der Rezeptwebseite**

Geben Sie die `extract.recipe`-Methode und das `none`-Ausweichverhalten an. Senden Sie auch ein `img`-Element, wobei das `data-render-src`-Attribut auf die Rezept-URL festgelegt ist. Wenn die API keinen Inhalt extrahieren kann, wird nur ein Snapshot der Rezeptwebseite gerendert.

Dieses Szenario bietet möglicherweise die meisten Informationen, da die Webseite weitere Informationen, wie z. B. Kundenbewertungen und Vorschläge, enthalten kann.

```html 
<div
    data-render-src="http://allrecipes.com/recipe/guacamole/"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<img data-render-src="http://allrecipes.com/recipe/guacamole/" />
```
 

**Extrahieren von Rezeptinformationen und Rendern eines Snapshots der Rezeptwebseite, wenn die Extraktion fehlschlägt**

Geben Sie die `extract.recipe`-Methode an, und verwenden Sie das standardmäßige Render-Ausweichverhalten. Wenn die API keinen Inhalt extrahieren kann, wird stattdessen ein Snapshot der Rezeptwebseite gerendert.

```html  
<div
    data-render-src="http://www.foodnetwork.com/recipes/alton-brown/creme-brulee-recipe.html"
    data-render-method="extract.recipe">
</div>
```


**Extrahieren von Rezeptinformationen und Rendern eines Links zum Rezept**

Geben Sie die `extract.recipe`-Methode und das `none`-Ausweichverhalten an. Senden Sie auch ein `a`-Element, wobei das `src`-Attribut auf die Rezept-URL festgelegt ist (Sie können alternativ auch andere Informationen senden, die Sie der Seite hinzufügen möchten). Wenn die API keinen Inhalt extrahieren kann, wird nur der Rezept-Link gerendert.

```html  
<div
    data-render-src="http://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<a href="http://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html">Recipe URL</a>
``` 


<a name="product"></a>
## <a name="product-listing-extractions"></a>Extraktionen von Produktlisten

- Titel
- Bewertung
- Primäres Bild
- Beschreibung
- Features
- Spezifikationen</td>

  ![Ein Beispiel für die Extraktion einer Produktliste.](images/product-extraction.png)

Die API ist für Produkte von vielen beliebten Websites wie *Amazon.com* und *HomeDepot.com* optimiert.

### <a name="common-scenarios-for-recipe-extractions"></a>Häufige Szenarien für Rezeptextraktionen

**Extrahieren von Produktinformationen und Rendern eines Snapshots der Produktwebseite**

Geben Sie die `extract.product`-Methode und das `none`-Ausweichverhalten an. Senden Sie auch ein `img`-Element, wobei das `data-render-src`-Attribut auf die Produkt-URL festgelegt ist. Wenn die API keinen Inhalt extrahieren kann, wird nur ein Snapshot der Produktwebseite gerendert.

Dieses Szenario bietet möglicherweise die meisten Informationen, da die Webseite weitere Informationen, wie z. B. Kundenbewertungen und Vorschläge, enthalten kann.

```html 
<div
    data-render-src="http://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<img data-render-src="http://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO" />
```


**Extrahieren von Produktinformationen und Rendern eines Snapshots der Produktwebseite, wenn die Extraktion fehlschlägt**

Geben Sie die `extract.product`-Methode an, und verwenden Sie das standardmäßige Render-Ausweichverhalten. Wenn die API keinen Inhalt extrahieren kann, wird stattdessen ein Snapshot der Produktwebseite gerendert.

```html 
<div
    data-render-src="http://www.sears.com/craftsman-19hp-42-8221-turn-tight-174-hydrostatic-yard-tractor/p-07120381000P"
    data-render-method="extract.product">
</div>
```
 

**Extrahieren von Produktinformationen und Rendern eines Links zum Produkt**

Geben Sie die `extract.product`-Methode und das `none`-Ausweichverhalten an. Senden Sie auch ein `a`-Element, wobei das `src`-Attribut auf die Produkt-URL festgelegt ist (Sie können alternativ auch andere Informationen senden, die Sie der Seite hinzufügen möchten). Wenn die API keinen Inhalt extrahieren kann, wird nur der Seitenlink gerendert.

```html 
<div
    data-render-src="http://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<a href="http://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001">Product URL</a>
```


<a name="unknown"></a> 
## <a name="unknown-content-type-extractions"></a>Extraktionen unbekannter Inhaltstypen

Wenn Sie den Inhaltstyp (Visitenkarte, Rezept oder Produkt), den Sie versenden möchten, nicht kennen, können Sie die unqualifizierte `extract`-Methode verwenden und die OneNote-API den Typ automatisch erkennen lassen. Dies ist möglicherweise sinnvoll, wenn Ihre App andere Erfassungstypen sendet.

> **Hinweis:** Wenn Sie den Inhaltstyp kennen, den Sie senden, verwenden Sie die Methode `extract.businesscard`, `extract.recipe` oder `extract.product`. In einigen Fällen kann dies hilfreich sein, um die Extraktionsergebnisse zu optimieren.
 
### <a name="common-scenarios-for-unknown-extractions"></a>Häufige Szenarien für Extraktionen unbekannter Inhaltstypen

**Senden Sie ein Bild oder eine URL, und rendern Sie das bereitgestellte Bild oder einen Snapshot der Webseite, wenn die Extraktion fehlschlägt**

Geben Sie die `extract`-Methode an, damit die API den Inhaltstyp automatisch erkennen kann und verwenden Sie das standardmäßige render-Ausweichverhalten. Wenn die API keinen Inhalt extrahieren kann, wird stattdessen das bereitgestellte Bild oder ein Snapshot der Webseite gerendert.

```html 
<div
    data-render-src="some image or url"
    data-render-method="extract">
</div>
```


<a name="request-response-info"></a>
## <a name="response-information"></a>Informationen in der Antwort

| Antwortdaten | Beschreibung |  
|------|------|  
| Erfolgscode | HTTP-Statuscode 201 für eine erfolgreiche POST-Anforderung, HTTP-Statuscode 204 für eine erfolgreiche PATCH-Anforderung. |  
| Fehler| Informationen zu OneNote-Fehlern, die Microsoft Graph zurückgeben kann, finden Sie unter [Fehlercodes für OneNote-APIs in Microsoft Graph](onenote_error_codes.md). |  


<a name="permissions"></a>
## <a name="permissions"></a>Berechtigungen

Zum Erstellen oder Aktualisieren von OneNote-Seiten müssen Sie die entsprechenden Berechtigungen anfordern. Wählen Sie die niedrigste Berechtigungsstufe, die Ihre App zur Erledigung ihrer Aufgaben benötigt.

**Berechtigungen für _POST Pages_**

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All  

**Berechtigungen für _PATCH Pages_**

- Notes.ReadWrite
- Notes.ReadWrite.All

Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie in der [Microsoft Graph-Berechtigungsreferenz](permissions_reference.md).


<a name="see-also"></a>
## <a name="additional-resources"></a>Weitere Ressourcen

- [Erstellen von OneNote-Seiten](onenote-create-page.md)
- [Aktualisieren mit OneNote-Seiteninhalt](onenote_update_page.md)
- [Hinzufügen von Bildern und Dateien](onenote_images_files.md)
- [Integrieren in OneNote](integrate_with_onenote.md)
- [OneNote-Entwicklerblog](http://go.microsoft.com/fwlink/?LinkID=390183)
- [Fragen zur OneNote-Entwicklung auf Stack Overflow](http://go.microsoft.com/fwlink/?LinkID=390182)
- [OneNote GitHub-Repos](http://go.microsoft.com/fwlink/?LinkID=390178)  

