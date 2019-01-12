---
title: Erstellen von absolut positionierten Elementen auf OneNote-Seiten
description: Das „body“-Element einer OneNote-Seite kann mehrere direkt untergeordnete Elemente des Typs `div`, `img` oder `object` enthalten, die unabhängig voneinander auf der Seite positioniert werden können.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 9630741091be52de8791f560a13b225ccce2e218
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981168"
---
# <a name="create-absolute-positioned-elements-in-onenote-pages"></a>Erstellen von absolut positionierten Elementen auf OneNote-Seiten

Das „body“-Element einer OneNote-Seite kann mehrere direkt untergeordnete Elemente des Typs `div`, `img` oder `object` enthalten, die unabhängig voneinander auf der Seite positioniert werden können.

<a name="attributes"></a>

## <a name="attributes-and-positioning-behavior"></a>Attribute und Positionierungsverhalten

Mithilfe der Attribute `data-absolute-enabled` und [`style`](#supported-css-style-attributes) können Sie absolut positionierte Elemente auf einer Seite erstellen. Dabei gilt:

- Das „body“-Element muss `data-absolute-enabled="true"` enthalten. Fehlt diese Eigenschaft oder ist sie auf `false` gesetzt, werden alle „body“-Inhalte in einem absolut positionierten „div“-Element `_default` gerendert, das von der API erstellt wird. Dabei werden alle Positionseinstellungen ignoriert.

- Nur Elemente des Typs `div`, `img` oder `object` können absolut positionierte Elemente sein. 

- Absolut positionierte Elemente müssen `style="position:absolute"` enthalten.

- Absolut positionierte Elemente müssen direkt untergeordnete Elemente des Elements `body` sein. Alle direkt untergeordneten Elemente des „body“-Elements, die keine absolut positionierten Elemente des Typs `div`, `img` oder `object` sind, werden als statische Inhalte innerhalb des absolut positionierten „div“-Elements `_default` gerendert.

- Absolut positionierte Elemente werden an den festgelegten oberen und linken Koordinaten relativ zur Startposition 0:0 in der linken oberen Ecke der Seite positioniert, über dem Titelbereich.

- Wenn für ein absolut positioniertes Element die obere Koordinate oder die linke Koordinate nicht angegeben ist, wird die fehlende Koordinate auf ihren jeweiligen Standardwert gesetzt: `top:120px` oder `left:48px`. Diese Standardkoordinaten legen eine Position direkt unter dem Titelbereich fest. Das Weglassen von Koordinaten kann dazu führen, dass Elemente übereinander gestapelt werden.

- Absolut positionierte Elemente können weder geschachtelt werden noch positionierte Elemente enthalten. Die API ignoriert alle für geschachtelte Elemente innerhalb eines absolut positionierten „div“-Elements angegebenen Positionseinstellungen, rendert die geschachtelten Inhalte innerhalb des absolut positionierten übergeordneten „div“-Elements und gibt eine Warnung in der Eigenschaft **api.diagnostics** in der Antwort zurück.


### <a name="example"></a>Beispiel

Das folgende Beispiel enthält ein direkt untergeordnetes Element des Typs `p`, ein absolut positioniertes „div“-Element und ein nicht absolut positioniertes „div“-Element.

#### <a name="input-html"></a>Eingabe-HTML  

   ```html 
   <body data-absolute-enabled="true">
       <p>This content will appear in the _default div.</p>
       <div style="position:absolute;top:175px;left:100px" data-id="div1">
         <p>This content will appear in an absolute positioned div.</p>
       </div>
       <div>
           <p>This content will also appear in the _default div.</p>
       </div>
   </body>
   ```

Die API rendert das nicht absolut positionierte „div“-Element im „div“-Element „default“. Beachten Sie: Die geschachtelten Tags des Typs `<div>` werden verworfen, da sie keine semantischen Informationen definieren (z. B. `data-id`).

#### <a name="output-html"></a>Ausgabe-HTML 

   ```html 
   <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11pt">
       <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
           <p>This content will appear in the _default div.</p>
           <p>This content will also appear in the _default div.</p>
       </div>
       <div data-id="div1" style="position:absolute;left:99px;top:174px;width:624px">
           <p>This content will appear in an absolute positioned div.</p>
       </div>
   </body>
   ```

### <a name="example"></a>Beispiel

Das folgende Beispiel erstellt eine Seite, die ein einziges absolut positioniertes „div“-Element und ein einziges absolut positioniertes Bild enthält.


#### <a name="input-html"></a>Eingabe-HTML  

```html 
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true">
        <div style="position:absolute;width:280px;top:120px;left:68px">
            <p>Some text</p>
            <img style="width:120px" src="https://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
            <div>
                <p>More text inside a regular, nested div</p>
            </div>
        </div>
        <img style="position:absolute;width:360px;top:350px;left:300px" src="https://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
    </body>
</html>
```
 
Die OneNote-API wertet den Eingabe-HTML-Code aus und behält alle semantischen Inhalte sowie alle strukturellen Informationen bei, die von OneNote unterstützt werden. Die daraus resultierende Seite wird wie in der Abbildung unten gerendert (ohne die sichtbaren Rahmen um das „div“-Element und das Bild). 

![Resultierende Seite mit absolut positioniertem „div“-Element und absolut positioniertem Bild](images/abs-pos.png)

Beachten Sie die Änderungen am nicht berücksichtigten, geschachtelten „div“-Element aus dem Eingabe-HTML-Code. Die API behält die Inhalte des „div“-Elements bei, verwirft jedoch die Tags des Typs `<div>`, weil das „div“-Element keine semantischen Informationen definiert (z. B. `data-id`).

Weitere Informationen dazu, wie die OneNote-API Eingabe-HTML und Ausgabe-HTML verarbeitet, finden Sie unter [Eingabe- und Ausgabe-HTML auf OneNote-Seiten](onenote-input-output-html.md).

<a name="style-attributes"></a>

## <a name="supported-css-style-attributes"></a>Unterstützte CSS-Formatattribute

Für alle absolut positionierten Elemente können eine obere Position und eine linke Position angegeben werden. Für „div“-Elemente und Bilder lässt sich die Breite, für Bilder zusätzlich auch die Höhe festlegen. Beispiel:

```html
<img style="position:absolute;top:140px;left:95px;width:480px;height:665px" src="..." />
```

| Attribut | Unterstütztes Element | Beschreibung |  
|:------|:------|:------|  
| top | div, img, object | Y-Koordinate des oberen Rands des Elements, anzugeben ausschließlich in Pixel. Der Standardwert ist 120 Pixel.<br/><br/>Beispiel: `top:140px` |  
| left |  div, img, object  | X-Koordinate des linken Rands des Elements, anzugeben ausschließlich in Pixel Der Standardwert ist 48 Pixel.<br/><br/>Beispiel: `left:95px` |  
| width |  div, img  | Die Breite des Elements, anzugeben ausschließlich in Pixel.<br/><br/>Beispiel: `width:480px` |  
| height | img | Die Höhe des Elements, anzugeben ausschließlich in Pixel. Die Höhe von „div“-Elementen wird zur Laufzeit berechnet; angegebene Höhenwerte werden ignoriert.<br/><br/>Beispiel: `height:665px` |  
 
Andere Positionsattribute, beispielsweise `z-index`, werden ignoriert. Für absolut positionierte Bilder können Sie entweder das Attribut `data-render-src` oder das Attribut `src` verwenden.


<a name="request-response-info"></a>

## <a name="response-information"></a>Informationen in der Antwort

Die OneNote-API gibt in der Antwort die nachfolgenden Informationen zurück.

| Antwortdaten | Beschreibung |  
|:------|:------|  
| Erfolgscode | HTTP-Statuscode 201 bei erfolgreich ausgeführter POST-Anforderung, HTTP-Statuscode 204 bei erfolgreich ausgeführter PATCH-Anforderung |  
| Fehler | Informationen zu OneNote-Fehlern, die Microsoft Graph zurückgeben kann, finden Sie unter [Fehlercodes für OneNote-APIs in Microsoft Graph](onenote-error-codes.md). |  
  


<a name="permissions"></a>

## <a name="permissions"></a>Berechtigungen

Zum Erstellen oder Aktualisieren von OneNote-Seiten müssen Sie die entsprechenden Berechtigungen anfordern. Wählen Sie die niedrigste Berechtigungsstufe, die Ihre App zur Erledigung ihrer Aufgaben benötigt.

#### <a name="permissions-for-post-pages"></a>Berechtigungen für BEITRAG-Seiten 

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All  


#### <a name="permissions-for-patch-pages"></a>Berechtigungen für PATCH-Seiten 

- Notes.ReadWrite
- Notes.ReadWrite.All

Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie unter [OneNote-Berechtigungsbereiche](permissions-reference.md#notes-permissions).


<a name="see-also"></a>

## <a name="see-also"></a>Siehe auch

- [Erstellen von OneNote-Seiten](onenote-create-page.md)
- [Aktualisieren der Inhalte von OneNote-Seiten](onenote-update-page.md)
- [Integrieren mit OneNote](integrate-with-onenote.md)
- [OneNote-Entwicklerblog](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Fragen zur OneNote-Entwicklung auf Stack Overflow](https://go.microsoft.com/fwlink/?LinkID=390182)
- [OneNote GitHub-Repos](https://go.microsoft.com/fwlink/?LinkID=390178)  

