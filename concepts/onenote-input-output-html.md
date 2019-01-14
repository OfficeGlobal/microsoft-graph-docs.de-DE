---
title: Eingabe- und Ausgabe-HTML auf OneNote-Seiten
description: 'Der HTML-Code, der den Seiteninhalt und die Seitenstruktur definiert, wenn Sie eine OneNote-Seite erstellen oder aktualisieren, wird *Eingabe-HTML* genannt. '
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 0cc2c0994a5e4d2a45e78c055af466f1c4999de6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981532"
---
# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="963da-103">Eingabe- und Ausgabe-HTML auf OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="963da-103">Input and output HTML in OneNote pages</span></span>

<span data-ttu-id="963da-104">Der HTML-Code, der den Seiteninhalt und die Seitenstruktur definiert, wenn Sie eine OneNote-Seite [erstellen](onenote-create-page.md) oder [aktualisieren](onenote-update-page.md), wird *Eingabe-HTML* genannt.</span><span class="sxs-lookup"><span data-stu-id="963da-104">The HTML that defines the page content and structure when you [create](onenote-create-page.md) or [update](onenote-update-page.md) a OneNote page is called *input HTML*.</span></span> 

<span data-ttu-id="963da-105">Der HTML-Code, der beim [Abrufen von Seiteninhalt](onenote-get-content.md) zurückgegeben wird, heißt *Ausgabe-HTML*.</span><span class="sxs-lookup"><span data-stu-id="963da-105">The HTML that's returned when you [get page content](onenote-get-content.md) is called *output HTML*.</span></span> <span data-ttu-id="963da-106">Der Ausgabe-HTML-Code entspricht nicht dem Eingabe-HTML-Code.</span><span class="sxs-lookup"><span data-stu-id="963da-106">Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="963da-107">Die OneNote-APIs in Microsoft Graph behalten den semantischen Inhalt und die grundlegende Struktur des Eingabe-HTML-Codes bei, konvertieren diese jedoch in [unterstützte HTML-Elemente und CSS-Eigenschaften](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span><span class="sxs-lookup"><span data-stu-id="963da-107">The OneNote APIs in Microsoft Graph preserve the semantic content and basic structure of the input HTML, but convert it to a set of [supported HTML elements and CSS properties](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span></span> <span data-ttu-id="963da-108">Die APIs fügen zudem benutzerdefinierte Attribute hinzu, die OneNote-Funktionen unterstützen.</span><span class="sxs-lookup"><span data-stu-id="963da-108">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="963da-109">Dieser Artikel beschreibt die wichtigsten Elemente und Attribute von Eingabe- und Ausgabe-HTML-Codes.</span><span class="sxs-lookup"><span data-stu-id="963da-109">This article describes the principal elements and attributes of input and output HTML.</span></span> <span data-ttu-id="963da-110">Es kann hilfreich sein, Eingabe-HTML-Codes zu verstehen, wenn Sie Seiteninhalte erstellen oder aktualisieren. Mit Ausgabe- HTML-Codes sollten Sie sich auskennen, wenn Sie zurückgegebene Seiteninhalte analysieren möchten.</span><span class="sxs-lookup"><span data-stu-id="963da-110">It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="963da-111">Textkörperelement</span><span class="sxs-lookup"><span data-stu-id="963da-111">body element</span></span>

<span data-ttu-id="963da-112">Der HTML-Inhalt im Textkörper der Seite repräsentiert den Seiteninhalt und die Seitenstruktur, einschließlich der Bild- und Dateiressourcen.</span><span class="sxs-lookup"><span data-stu-id="963da-112">The HTML content in the page body represents the page content and structure, including image and file resources.</span></span> <span data-ttu-id="963da-113">Das **body**-Element kann die folgenden Attribute in der Eingabe- und Ausgabe-HTML enthalten.</span><span class="sxs-lookup"><span data-stu-id="963da-113">The **body** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="963da-114">Eingabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-114">Input attributes</span></span>

|<span data-ttu-id="963da-115">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-115">Input attribute</span></span>|<span data-ttu-id="963da-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-116">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-117">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="963da-117">data-absolute-enabled</span></span> | <span data-ttu-id="963da-118">Gibt an, ob der Eingabe-Textkörper [absolute positioned](onenote-abs-pos.md)-Elemente unterstützt.</span><span class="sxs-lookup"><span data-stu-id="963da-118">Indicates whether the input body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> |
| <span data-ttu-id="963da-119">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="963da-119">style</span></span> | <p><span data-ttu-id="963da-120">Die CSS-[style](#styles)-Eigenschaften des Textkörpers.</span><span class="sxs-lookup"><span data-stu-id="963da-120">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="963da-121">In der Ausgabe-HTML können Eingabeeinstellungen eingebettet in die entsprechenden untergeordneten Elemente zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="963da-121">In the output HTML, input settings might be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="963da-122">Hintergrundfarbe wird derzeit nicht für das **body**-Element unterstützt.</span><span class="sxs-lookup"><span data-stu-id="963da-122">Background color is not currently supported for the **body** element.</span></span></p> |
 

#### <a name="output-attributes"></a><span data-ttu-id="963da-123">Ausgabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-123">Output attributes</span></span>

|<span data-ttu-id="963da-124">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-124">Output attribute</span></span>|<span data-ttu-id="963da-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-125">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-126">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="963da-126">data-absolute-enabled</span></span> | <span data-ttu-id="963da-127">Gibt an, ob der Textkörper [absolute positioned](onenote-abs-pos.md)-Elemente unterstützt.</span><span class="sxs-lookup"><span data-stu-id="963da-127">Indicates whether the body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> <span data-ttu-id="963da-128">Immer **true** in der HTML-Ausgabe.</span><span class="sxs-lookup"><span data-stu-id="963da-128">Always **true** in output HTML.</span></span> |
| <span data-ttu-id="963da-129">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="963da-129">style</span></span> | <span data-ttu-id="963da-130">Die Eigenschaften **font-family** und **font-size** des Textkörpers.</span><span class="sxs-lookup"><span data-stu-id="963da-130">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="963da-131">Div-Elemente</span><span class="sxs-lookup"><span data-stu-id="963da-131">div elements</span></span>

<span data-ttu-id="963da-132">**Div**-Elemente enthalten Text, Bilder und andere Inhalte.</span><span class="sxs-lookup"><span data-stu-id="963da-132">**Div** elements contain text, images, and other content.</span></span> <span data-ttu-id="963da-133">Das **div**-Element kann die folgenden Attribute in der Eingabe- und Ausgabe-HTML enthalten.</span><span class="sxs-lookup"><span data-stu-id="963da-133">A **div** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="963da-134">Eingabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-134">Input attributes</span></span>

|<span data-ttu-id="963da-135">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-135">Input attribute</span></span>|<span data-ttu-id="963da-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-136">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-137">data-id</span><span class="sxs-lookup"><span data-stu-id="963da-137">data-id</span></span> | <span data-ttu-id="963da-138">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-138">A reference for the element.</span></span><br/><br/><span data-ttu-id="963da-139">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-139">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-140">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="963da-140">data-render-fallback</span></span> | <span data-ttu-id="963da-141">Die Ausweichaktion bei einem Fehler der [Extraktion](onenote-extract-data.md): **render** (Standard) oder **none**.</span><span class="sxs-lookup"><span data-stu-id="963da-141">The fallback action if the [extraction](onenote-extract-data.md) fails: **render** (default) or **none**</span></span> |
| <span data-ttu-id="963da-142">data-render-method</span><span class="sxs-lookup"><span data-stu-id="963da-142">data-render-method</span></span> | <span data-ttu-id="963da-143">Die auszuführende [Extraktionsmethode](onenote-extract-data.md), z. B.:</span><span class="sxs-lookup"><span data-stu-id="963da-143">The [extraction](onenote-extract-data.md) method to perform, for example:</span></span><br/><span data-ttu-id="963da-144">`extract.businesscard` oder `extract.recipe`</span><span class="sxs-lookup"><span data-stu-id="963da-144">`extract.businesscard` or `extract.recipe`</span></span> |
| <span data-ttu-id="963da-145">data-render-src</span><span class="sxs-lookup"><span data-stu-id="963da-145">data-render-src</span></span> | <span data-ttu-id="963da-146">Die Inhaltsquelle für die [Extraktion](onenote-extract-data.md).</span><span class="sxs-lookup"><span data-stu-id="963da-146">The content source for the [extraction](onenote-extract-data.md).</span></span> |
| <span data-ttu-id="963da-147">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="963da-147">style</span></span> | <span data-ttu-id="963da-148">Die Position, Größe, Schriftart und Farbe von Eigenschaften für div:</span><span class="sxs-lookup"><span data-stu-id="963da-148">The position, size, font, and color properties for the div:</span></span> <ul><li><span data-ttu-id="963da-149">**Position** (nur **absolut**), **links**, **oben** und **Breite** (Höhe wird für div-Tags automatisch konfiguriert)</span><span class="sxs-lookup"><span data-stu-id="963da-149">**position** (**absolute** only), **left**, **top**, and **width** (height is auto-configured for divs)</span></span><br/><br/><span data-ttu-id="963da-150">Wird verwendet, um ein [absolut positioniertes](onenote-abs-pos.md)-Div-Element zu erstellen, wenn das Div-Element ein direktes untergeordnetes Element des Textkörpers und für den Textkörper `data-absolute-enabled="true"` angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="963da-150">Used to create an [absolute positioned](onenote-abs-pos.md) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="963da-151">Beispiel: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="963da-151">Example: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></li><li><span data-ttu-id="963da-p108">Die CSS-[style](#styles)-Eigenschaften des Elements. In der Ausgabe-HTML werden diese Werte inline in entsprechenden untergeordneten Elementen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="963da-p108">The CSS [style](#styles) properties of the element. In the output HTML, these values are returned inline on appropriate child elements.</span></span></li></ul> |
 

<span data-ttu-id="963da-154">Die OneNote-APIs in Microsoft Graph umschließen alle Textkörper mit mindestens einem Div.</span><span class="sxs-lookup"><span data-stu-id="963da-154">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="963da-155">Die API erstellt ein standardmäßiges Div (mit `data-id="_default"`-Attributen), die den Textkörper enthalten, wenn:</span><span class="sxs-lookup"><span data-stu-id="963da-155">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="963da-156">Das **data-absolute-enabled**-Attribut des Eingabe-Textkörper-Elements ausgelassen oder auf **false** gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="963da-156">The input body element's **data-absolute-enabled** attribute is omitted or set to **false**.</span></span> <span data-ttu-id="963da-157">In diesem Fall werden alle Inhalte des Textkörpers im standardmäßigen Div abgelegt.</span><span class="sxs-lookup"><span data-stu-id="963da-157">In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="963da-158">Das **data-absolute-enabled**-Attribut des Eingabe-Textkörper-Elements auf **true** gesetzt wird, die Eingabe HTML jedoch direkt untergeordnete Elemente enthält, die [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img** oder **object**-Elemente sind.</span><span class="sxs-lookup"><span data-stu-id="963da-158">The input body element's **data-absolute-enabled** attribute is **true**, but the input HTML contains direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements.</span></span> <span data-ttu-id="963da-159">In diesem Fall werden untergeordnete Elemente, die keine [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img** oder **object**-Elemente sind, im standardmäßigen Div abgelegt.</span><span class="sxs-lookup"><span data-stu-id="963da-159">In this case, direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


#### <a name="output-attributes"></a><span data-ttu-id="963da-160">Ausgabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-160">Output attributes</span></span>

|<span data-ttu-id="963da-161">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-161">Output attribute</span></span>|<span data-ttu-id="963da-162">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-162">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-163">data-id</span><span class="sxs-lookup"><span data-stu-id="963da-163">data-id</span></span> | <span data-ttu-id="963da-164">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-164">A reference for the element.</span></span><br/><br/><span data-ttu-id="963da-165">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-165">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-166">id</span><span class="sxs-lookup"><span data-stu-id="963da-166">id</span></span> | <span data-ttu-id="963da-167">Eine eindeutige generierte ID für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-167">A unique, generated ID for the element.</span></span> <span data-ttu-id="963da-168">Zurückgegeben von einem [GET requests to a page's *-content*-Endpunkt ](/graph/api/page-get?view=graph-rest-1.0), wenn die `includeIDs=true`-Abfrageoption verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="963da-168">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="963da-169">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-169">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-170">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="963da-170">style</span></span> | <span data-ttu-id="963da-171">Die Positions- und Größeneigenschaften des div-Elements.</span><span class="sxs-lookup"><span data-stu-id="963da-171">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="963da-172">Nicht beitragende Divs</span><span class="sxs-lookup"><span data-stu-id="963da-172">Non-contributing divs</span></span>

<span data-ttu-id="963da-173">Wenn ein **div**-Element in der Eingabe-HTML nichts zur Seitenstruktur beiträgt und keine von OneNote verwendeten Informationen enthält,  verschiebt die API den Inhalt des div-Elements in das übergeordnete oder standardmäßige div-Element.</span><span class="sxs-lookup"><span data-stu-id="963da-173">When a **div** element in the input HTML does not contribute to the page structure or carry information that OneNote uses, the API moves the div's content into the parent or default div.</span></span> <span data-ttu-id="963da-174">Dieser Vorgang wird in den folgenden Beispielen dargestellt.</span><span class="sxs-lookup"><span data-stu-id="963da-174">This is illustrated in the following examples.</span></span>

#### <a name="input-html"></a><span data-ttu-id="963da-175">Eingabe-HTML</span><span class="sxs-lookup"><span data-stu-id="963da-175">Input HTML</span></span>

<span data-ttu-id="963da-176">Enthält ein nicht beitragendes, geschachteltes div-Element.</span><span class="sxs-lookup"><span data-stu-id="963da-176">Contains a non-contributing, nested div.</span></span>

```html
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body>
        <div>
            <p>Some text</p>
            <div>
                <p>More text inside a div that doesn't define page structure</p>
            </div>
        </div>
    </body>
</html>
```

#### <a name="output-html"></a><span data-ttu-id="963da-177">Ausgabe-HTML</span><span class="sxs-lookup"><span data-stu-id="963da-177">Output HTML</span></span>

> <span data-ttu-id="963da-178">**Hinweis:** Der DIV-Inhalt wurde in die übergeordnete Div verschoben, und die geschachtelten `<div>`-Tags wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="963da-178">**Note:** The div's content was moved to the parent div and the nested `<div>` tags have been removed.</span></span> <span data-ttu-id="963da-179">Die Div wäre erhalten geblieben, wenn sie semantische Informationen definiert hätte, z. B. eine **Daten-Id** (Beispiel: `<div data-id="keep-me">`).</span><span class="sxs-lookup"><span data-stu-id="963da-179">The div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

```html
<html htmlns="https://www.w3.org/1999/xhtml" lang="en-US">
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11px">
        <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
            <p>Some text</p>
            <p>More text inside a nested div</p>
        </div>
    </body>
</html>
```


## <a name="img-elements"></a><span data-ttu-id="963da-180">img-Elemente</span><span class="sxs-lookup"><span data-stu-id="963da-180">img elements</span></span>

<span data-ttu-id="963da-181">Bilder auf OneNote-Seiten werden durch **img**-Elemente dargestellt.</span><span class="sxs-lookup"><span data-stu-id="963da-181">Images on OneNote pages are represented by **img** elements.</span></span> <span data-ttu-id="963da-182">Das **img**-Element kann die folgenden Attribute in der Eingabe- und Ausgabe-HTML enthalten.</span><span class="sxs-lookup"><span data-stu-id="963da-182">An **img** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="963da-183">Eingabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-183">Input attributes</span></span>

|<span data-ttu-id="963da-184">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-184">Input attribute</span></span>|<span data-ttu-id="963da-185">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-185">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-186">alt</span><span class="sxs-lookup"><span data-stu-id="963da-186">alt</span></span> | <span data-ttu-id="963da-187">Der angegebene Alternativtext für das Bild.</span><span class="sxs-lookup"><span data-stu-id="963da-187">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="963da-188">data-id</span><span class="sxs-lookup"><span data-stu-id="963da-188">data-id</span></span> | <span data-ttu-id="963da-189">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-189">A reference for the element.</span></span><br/><br/><span data-ttu-id="963da-190">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-190">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-191">data-render-src</span><span class="sxs-lookup"><span data-stu-id="963da-191">data-render-src</span></span> |<span data-ttu-id="963da-192">Es ist entweder **data-render-src** oder **src** erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="963da-192">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="963da-193">Die Webseite, die als Bitmapbild auf der OneNote-Seite gerendert werden soll:</span><span class="sxs-lookup"><span data-stu-id="963da-193">The webpage to render as a bit-mapped image on the OneNote page:</span></span><br/><br/> <span data-ttu-id="963da-194">- `data-render-src="https://..."` für eine öffentliche URL.</span><span class="sxs-lookup"><span data-stu-id="963da-194">- `data-render-src="https://..."` for a public URL.</span></span><br/><br/> <span data-ttu-id="963da-195">- `data-render-src="name:BlockName"` für ein Bild-Bestandteil im Block "Präsentation" einer [mehrteiligen Anforderung](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span><span class="sxs-lookup"><span data-stu-id="963da-195">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span><br/><br/><span data-ttu-id="963da-196">Diese Methode ist nützlich, wenn die Webseite so komplex ist, dass sie nicht zuverlässig von OneNote analysiert werden kann, oder wenn für die Seite eine Anmeldung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="963da-196">This method is useful when the webpage is more complex than the OneNote page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="963da-197">data-tag</span><span class="sxs-lookup"><span data-stu-id="963da-197">data-tag</span></span> | <span data-ttu-id="963da-198">Ein [Notiztag](onenote-note-tags.md) für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-198">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="963da-199">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="963da-199">style</span></span> |<span data-ttu-id="963da-200">Die Position- und Größen-Eigenschaften für das Bild: **Position** (nur **absolute**), **links**, **oben**, **Breite** und **Höhe**.</span><span class="sxs-lookup"><span data-stu-id="963da-200">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="963da-201">Die Größe kann für jedes Bild festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="963da-201">Size can be set on any image.</span></span><br/><br/><span data-ttu-id="963da-202">Positionseigenschaften werden verwendet, um ein [absolute positioned](onenote-abs-pos.md)-Bild zu erstellen, wenn das Bild ein direktes untergeordnetes Element des Textkörpers und für den Textkörper `data-absolute-enabled="true"` angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="963da-202">Position properties are used to create an [absolute positioned](onenote-abs-pos.md) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="963da-203">Beispiel: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="963da-203">Example: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="963da-204">In der Ausgabe-HTML wird die Bildgröße separat in **width**- und **height**-Attributen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="963da-204">In the output HTML, the image size is returned separately in **width** and **height** attributes.</span></span> |
| <span data-ttu-id="963da-205">src</span><span class="sxs-lookup"><span data-stu-id="963da-205">src</span></span> |<span data-ttu-id="963da-206">Es ist entweder **src** oder **data-render-src** erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="963da-206">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="963da-207">Das Bild, das auf der OneNote-Seite gerendert werden soll:</span><span class="sxs-lookup"><span data-stu-id="963da-207">The image to render on the OneNote page:</span></span><br/><br/><span data-ttu-id="963da-208">- `src="https://..."` für eine URL zu einem öffentlich verfügbaren Bild im Internet.</span><span class="sxs-lookup"><span data-stu-id="963da-208">- `src="https://..."` for a URL to a publicly available image on the Internet.</span></span><br/><br/> <span data-ttu-id="963da-209">- `src="name:BlockName"` für einen benannten Teil in einer mehrteiligen Anforderung, die das Bild darstellt.</span><span class="sxs-lookup"><span data-stu-id="963da-209">- `src="name:BlockName"` for a named part in a multipart request that represents the image.</span></span>|
| <span data-ttu-id="963da-210">Breite, Höhe</span><span class="sxs-lookup"><span data-stu-id="963da-210">width, height</span></span> | <span data-ttu-id="963da-211">Die Breite oder Höhe des Bilds, in Pixel, aber ohne px.</span><span class="sxs-lookup"><span data-stu-id="963da-211">The width or height of the image, in pixels but without the px.</span></span> <span data-ttu-id="963da-212">Beispiel: `width="400"`</span><span class="sxs-lookup"><span data-stu-id="963da-212">Example: `width="400"`</span></span> |
 
> <span data-ttu-id="963da-213">**Hinweis:** Die OneNote-APIs erkennt automatisch den Eingabe-Bildtyp und gibt ihn als **data-fullres-src-type** an die Ausgabe-HTML zurück.</span><span class="sxs-lookup"><span data-stu-id="963da-213">**Note:** The OneNote APIs automatically detect the input image type, and return it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="963da-214">Daneben gibt die API auch den Bildtyp des optimierten Bilds zurück, in **data-src-type**.</span><span class="sxs-lookup"><span data-stu-id="963da-214">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

#### <a name="output-attributes"></a><span data-ttu-id="963da-215">Ausgabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-215">Output attributes</span></span>

|<span data-ttu-id="963da-216">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-216">Output attribute</span></span>|<span data-ttu-id="963da-217">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-217">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-218">alt</span><span class="sxs-lookup"><span data-stu-id="963da-218">alt</span></span> | <span data-ttu-id="963da-219">Der angegebene Alternativtext für das Bild.</span><span class="sxs-lookup"><span data-stu-id="963da-219">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="963da-220">data-id</span><span class="sxs-lookup"><span data-stu-id="963da-220">data-id</span></span> | <span data-ttu-id="963da-221">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-221">A reference for the element.</span></span><br/><br/><span data-ttu-id="963da-222">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-222">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-223">data-index</span><span class="sxs-lookup"><span data-stu-id="963da-223">data-index</span></span> | <span data-ttu-id="963da-p118">Die Position des Bilds. Für die Unterstützung von [geteilten Bildern](#split-images).</span><span class="sxs-lookup"><span data-stu-id="963da-p118">The position of the image. For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="963da-226">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="963da-226">data-fullres-src</span></span> | <span data-ttu-id="963da-227">Der Endpunkt für die Version der Bildressource, die ursprünglich in die Seite eingebettet war.</span><span class="sxs-lookup"><span data-stu-id="963da-227">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="963da-228">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="963da-228">data-fullres-src-type</span></span> | <span data-ttu-id="963da-229">Der Medientyp der **data-fullres-src**-Ressource. Beispiel: `image/png` oder `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="963da-229">The media type of the **data-fullres-src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="963da-230">data-options</span><span class="sxs-lookup"><span data-stu-id="963da-230">data-options</span></span> | <span data-ttu-id="963da-p119">Der Quelltyp: **printout** für PDF-Dateien oder **splitimage** für alle anderen. Gilt nur für [geteilte Bilder](#split-images), die mit dem **data-render-src**-Attribut erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="963da-p119">The source type: **printout** for PDF files or **splitimage** for all others. Applies only to [split images](#split-images) created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="963da-233">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="963da-233">data-render-original-src</span></span> | <span data-ttu-id="963da-234">Die ursprüngliche URL des Bilds, wenn das Quellbild aus dem öffentlichen Internet stammt und mit dem **data-render-src**-Attribut erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="963da-234">The original source URL of the image, if the source image is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="963da-235">data-src-type</span><span class="sxs-lookup"><span data-stu-id="963da-235">data-src-type</span></span> | <span data-ttu-id="963da-236">Der Medientyp der **src**-Ressource. Beispiel: `image/png` oder `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="963da-236">The media type of the **src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="963da-237">data-tag</span><span class="sxs-lookup"><span data-stu-id="963da-237">data-tag</span></span> | <span data-ttu-id="963da-238">Ein [Notiztag](onenote-note-tags.md) für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-238">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="963da-239">id</span><span class="sxs-lookup"><span data-stu-id="963da-239">id</span></span> | <span data-ttu-id="963da-240">Eine eindeutige generierte ID für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-240">A unique, generated ID for the element.</span></span> <span data-ttu-id="963da-241">Zurückgegeben von einem [GET requests to a page's *-content*-Endpunkt ](/graph/api/page-get?view=graph-rest-1.0), wenn die `includeIDs=true`-Abfrageoption verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="963da-241">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="963da-242">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-242">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-243">src</span><span class="sxs-lookup"><span data-stu-id="963da-243">src</span></span> | <span data-ttu-id="963da-244">Der Endpunkt für die Version der Bildressource, die für Webbrowser sowie mobile Geräte und Tablets optimiert wurde.</span><span class="sxs-lookup"><span data-stu-id="963da-244">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="963da-245">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="963da-245">style</span></span> | <span data-ttu-id="963da-246">Die Positionseigenschaften des Bilds.</span><span class="sxs-lookup"><span data-stu-id="963da-246">The position properties of the image.</span></span> |
| <span data-ttu-id="963da-247">width, height</span><span class="sxs-lookup"><span data-stu-id="963da-247">width, height</span></span> | <span data-ttu-id="963da-248">Die Breite oder Höhe des Bilds in Pixel.</span><span class="sxs-lookup"><span data-stu-id="963da-248">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="963da-249">Beispiele für die Ausgabe-HTML für Bilder</span><span class="sxs-lookup"><span data-stu-id="963da-249">Output HTML examples for images</span></span>

<span data-ttu-id="963da-250">Ausgabe-**img**-Elemente enthalten die Endpunkte für Bilddateiressourcen und den Bildtyp (siehe  unten).</span><span class="sxs-lookup"><span data-stu-id="963da-250">Output **img** elements contain endpoints for image file resources and the image type, as shown below.</span></span> <span data-ttu-id="963da-251">Sie können separate [GET-Anforderung zu Bildressourcen-Endpunkten](/graph/api/resource-get?view=graph-rest-1.0) durchführen, um die binäre Inhalt abzurufen.</span><span class="sxs-lookup"><span data-stu-id="963da-251">You can make separate [GET requests to image resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="963da-252">Standardmäßig können Bilder nicht direkt in einem Browser gerendert werden, da sie wie die restlichen Seiteninhalte privat sind und eine Autorisierung erforderlich ist, um sie abzurufen.</span><span class="sxs-lookup"><span data-stu-id="963da-252">By default, images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> <span data-ttu-id="963da-253">Um Öffentliche URLs für die Bildressourcen auf einer Seite zu erhalten, fügen Sie **preAuthenticated=true** in die Abfragezeichenfolge ein, wenn Sie die Seiteninhalte abrufen (Beispiel: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span><span class="sxs-lookup"><span data-stu-id="963da-253">To get public URLs to the image resources on a page, include **preAuthenticated=true** in the query string when you retrieve the page content (example: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span></span> <span data-ttu-id="963da-254">Die öffentlichen URLs, die zurückgegeben werden, sind eine Stunde lang gültig.</span><span class="sxs-lookup"><span data-stu-id="963da-254">The public URLs that are returned are valid for one hour.</span></span> 

#### <a name="image-with-public-url-when-preauthenticatedtrue-is-included-in-the-request"></a><span data-ttu-id="963da-255">Bild mit öffentlichen URL, wenn _vorauthentifiziert = True_ in der Anfrage enthalten ist</span><span class="sxs-lookup"><span data-stu-id="963da-255">Image with public URL when _preAuthenticated=true_ is included in the request</span></span>

```html
<img 
    width="170" height="128" 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-src-type="image/{type}" 
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-fullres-src-type="image/{type}"
/>
```

<span data-ttu-id="963da-256">Die folgenden Beispiele zeigen, welche Informationen ein **img**-Element in der Ausgabe-HTML enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="963da-256">The following examples show the information an **img** element might contain in the output HTML.</span></span>

#### <a name="image-with-web-ready-and-high-resolution-resources"></a><span data-ttu-id="963da-257">Bild mit webfähigen Ressourcen in hoher Auflösung</span><span class="sxs-lookup"><span data-stu-id="963da-257">Image with web-ready and high resolution resources</span></span>

```html
<img
    src="{web-ready-image-resource-url}/$value"
    data-src-type="image/{type}"
    data-fullres-src="{high-resolution-image-resource-url}/$value"
    data-fullres-src-type="image/{type}"
    [data-render-original-src="{original-source-url-or-named-part}"]
    [data-id="{image-id}"]
    [alt="supplied alt text"]
    [width="345"] [height="180"]
    [style="..."] />
```

#### <a name="image-created-by-using-the-data-render-src-attribute"></a><span data-ttu-id="963da-258">Mit dem *data-render-src*-Attribut erstelltes Bild</span><span class="sxs-lookup"><span data-stu-id="963da-258">Image created by using the *data-render-src* attribute</span></span>

```html
<img
    src="{web-ready-image-resource-url}/$value"
    data-src-type="image/{type}"
    data-fullres-src="{high-resolution-image-resource-url}/$value"
    data-fullres-src-type="image/{type}"
    data-render-original-src="{original-source-url-or-named-part}"
    [data-id="{image-id}"]
    [data-index="{index-of-split-image}"]
    [data-options="{printout-or-splitimage}"]
    [alt="supplied alt text"]
    [width="1024"] [height="1900"]
    [style="..."] />
```

### <a name="split-images"></a><span data-ttu-id="963da-259">Aufteilen von Bildern</span><span class="sxs-lookup"><span data-stu-id="963da-259">Split images</span></span>

<span data-ttu-id="963da-260">Bilder, die mit dem **data-render-src**-Attribut (aus einer Webseiten-URL oder einem benannten Teil) erstellt werden, werden für eine bessere Leistung und ein besseres Rendering möglicherweise in aus mehreren Komponenten bestehende Bilder aufgeteilt.</span><span class="sxs-lookup"><span data-stu-id="963da-260">Images that are created using the **data-render-src** attribute (from a webpage URL or a named part) might be split into multiple component images for performance and rendering reasons.</span></span> <span data-ttu-id="963da-261">Komponenten-Bildern wird allen der gleiche **data-id**-Wert zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="963da-261">Component images are all assigned the same **data-id** value.</span></span> <span data-ttu-id="963da-262">Jedes Komponenten-Bild verfügt über ein nullbasiertes data-index-Attribut, welches das ursprüngliche vertikale Layout definiert.</span><span class="sxs-lookup"><span data-stu-id="963da-262">Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

#### <a name="split-image-with-three-component-images"></a><span data-ttu-id="963da-263">Aufgeteiltes Bild mit drei Komponentenbildern</span><span class="sxs-lookup"><span data-stu-id="963da-263">Split image with three component images</span></span>

```html
<div data-id="multi-component-image" style="position:absolute;left:48px;top:120px;width:624px">
    <img
        src="{image-resource0-url}/$value"
        data-src-type="image/{type}"
        data-fullres-src="{image-resource0-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="0" 
        data-render-original-src="{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
    <img 
        src="{image-resource1-url}/$value" 
        data-src-type="image/{type}" 
        data-fullres-src="{image-resource1-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="1" 
        data-render-original-src="{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
    <img 
        src="{image-resource2-url}/$value" 
        data-src-type="image/{type}" 
        data-fullres-src="{image-resource2-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="2" 
        data-render-original-src=""{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
</div>
```

<span data-ttu-id="963da-264">Da Benutzer die Bilder auf der Seite verschieben können, werden die Indizes möglicherweise in falscher Reihenfolge zurückgegebenen.</span><span class="sxs-lookup"><span data-stu-id="963da-264">Because users can move the images on the page, the returned indexes might be out of order.</span></span> <span data-ttu-id="963da-265">Die Sortierung erfolgt normalerweise von oben nach unten auf der Y-Achse und von links nach rechts auf der X-Achse, wenn es Konflikte mit der Y-Sortierung gibt.</span><span class="sxs-lookup"><span data-stu-id="963da-265">Ordering should be in top to bottom y-order, and then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="963da-266">iframe-Elemente</span><span class="sxs-lookup"><span data-stu-id="963da-266">iframe elements</span></span>

<span data-ttu-id="963da-267">OneNote-Seiten können eingebettete Videos enthalten, die durch **iframe**-Elemente dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="963da-267">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

> <span data-ttu-id="963da-268">**Hinweis:** Sie können auch [eine Videodatei mithilfe eines **object**-Elements](onenote-images-files.md#adding-files) anfügen.</span><span class="sxs-lookup"><span data-stu-id="963da-268">**Note:** You can also [attach a video file using an **object** element](onenote-images-files.md#adding-files).</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="963da-269">Eingabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-269">Input attributes</span></span>

|<span data-ttu-id="963da-270">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-270">Input attribute</span></span>|<span data-ttu-id="963da-271">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-271">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-272">data-original-src</span><span class="sxs-lookup"><span data-stu-id="963da-272">data-original-src</span></span> | <span data-ttu-id="963da-273">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="963da-273">Required.</span></span> <span data-ttu-id="963da-274">Die URL der Videoquelle.</span><span class="sxs-lookup"><span data-stu-id="963da-274">The URL of the video source.</span></span> <span data-ttu-id="963da-275">Siehe [Liste der unterstützten Videoquellen](onenote-images-files.md#adding-videos).</span><span class="sxs-lookup"><span data-stu-id="963da-275">See the [list of supported video sources](onenote-images-files.md#adding-videos).</span></span> <br/><br/><span data-ttu-id="963da-276">Beispiel: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="963da-276">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="963da-277">Breite, Höhe</span><span class="sxs-lookup"><span data-stu-id="963da-277">width, height</span></span> | <span data-ttu-id="963da-278">Die Breite oder Höhe des iframe in Pixel.</span><span class="sxs-lookup"><span data-stu-id="963da-278">The width or height of the iframe, in pixels.</span></span> <span data-ttu-id="963da-279">Beispiel: `width=300`</span><span class="sxs-lookup"><span data-stu-id="963da-279">Example: `width=300`</span></span> |

#### <a name="output-attributes"></a><span data-ttu-id="963da-280">Ausgabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-280">Output attributes</span></span>

|<span data-ttu-id="963da-281">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-281">Output attribute</span></span>|<span data-ttu-id="963da-282">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-282">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-283">data-original-src</span><span class="sxs-lookup"><span data-stu-id="963da-283">data-original-src</span></span> | <span data-ttu-id="963da-284">Die URL der Videoquelle.</span><span class="sxs-lookup"><span data-stu-id="963da-284">The URL of the video source.</span></span> |
| <span data-ttu-id="963da-285">src</span><span class="sxs-lookup"><span data-stu-id="963da-285">src</span></span> | <span data-ttu-id="963da-286">Ein Link zu dem Video, das in die OneNote-Seite eingebettet ist.</span><span class="sxs-lookup"><span data-stu-id="963da-286">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="963da-287">Breite, Höhe</span><span class="sxs-lookup"><span data-stu-id="963da-287">width, height</span></span> | <span data-ttu-id="963da-288">Die Breite oder Höhe des iframe in Pixel.</span><span class="sxs-lookup"><span data-stu-id="963da-288">The width or height of the iframe, in pixels.</span></span><br/><br/><span data-ttu-id="963da-289">Beispiel: `width=300`</span><span class="sxs-lookup"><span data-stu-id="963da-289">Example: `width=300`</span></span> |
 
### <a name="output-html-example-for-videos"></a><span data-ttu-id="963da-290">Beispiel für eine Ausgabe-HTML eines Videos</span><span class="sxs-lookup"><span data-stu-id="963da-290">Output HTML example for videos</span></span>

<span data-ttu-id="963da-291">Ausgabe-**iframe**-Elemente enthalten Endpunkte, die wie dargestellt auf die Quellseite und das Video verweisen.</span><span class="sxs-lookup"><span data-stu-id="963da-291">Output **iframe** elements contain endpoints that link to the source page and video, as shown.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="963da-292">Object-Elemente</span><span class="sxs-lookup"><span data-stu-id="963da-292">object elements</span></span>

<span data-ttu-id="963da-293">OneNote-Seiten können Dateianlagen enthalten, die durch **object**-Elemente dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="963da-293">OneNote pages can contain file attachments represented by **object** elements.</span></span> <span data-ttu-id="963da-294">Das **object**-Element kann die folgenden Attribute in der Eingabe- und Ausgabe-HTML enthalten.</span><span class="sxs-lookup"><span data-stu-id="963da-294">An **object** element can contain the following attributes in the input and output HTML.</span></span>

> <span data-ttu-id="963da-295">**Hinweis:** OneNote-APIs können auch Dateiinhalte als Bilder auf einer Seite rendern, wenn die Datei als Bild gesendet und das Attribut **data-render-src** verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="963da-295">**Note:** The OneNote APIs can also render file content as images in a page when the file is sent as an image and uses the **data-render-src** attribute.</span></span>
> <span data-ttu-id="963da-296">Beispiel: `<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="963da-296">Example: `<img data-render-src="name:part-name" ... />`</span></span>
 

#### <a name="input-attributes"></a><span data-ttu-id="963da-297">Eingabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-297">Input attributes</span></span>

|<span data-ttu-id="963da-298">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-298">Input attribute</span></span>|<span data-ttu-id="963da-299">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-299">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-300">data</span><span class="sxs-lookup"><span data-stu-id="963da-300">data</span></span> | <span data-ttu-id="963da-301">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="963da-301">Required.</span></span> <span data-ttu-id="963da-302">Der Name des Teils, der die Datei in der [mehrteiligen Anforderung](/graph/api/section-post-pages?view=graph-rest-1.0#example) darstellt.</span><span class="sxs-lookup"><span data-stu-id="963da-302">The name of the part that represents the file in the [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span> |
| <span data-ttu-id="963da-303">data-attachment</span><span class="sxs-lookup"><span data-stu-id="963da-303">data-attachment</span></span> | <span data-ttu-id="963da-p130">Erforderlich. Der Dateiname.</span><span class="sxs-lookup"><span data-stu-id="963da-p130">Required. The file name.</span></span> |
| <span data-ttu-id="963da-306">data-id</span><span class="sxs-lookup"><span data-stu-id="963da-306">data-id</span></span> | <span data-ttu-id="963da-307">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-307">A reference for the element.</span></span><br/><br/><span data-ttu-id="963da-308">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-308">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-309">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="963da-309">style</span></span> | <span data-ttu-id="963da-310">Die Position- und Größen-Eigenschaften für das Objekt: **Position** (nur **absolute**), **links**, **oben** und **Breite**.</span><span class="sxs-lookup"><span data-stu-id="963da-310">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span><br/><br/><span data-ttu-id="963da-311">Wird verwendet, um ein [absolut positioniertes](onenote-abs-pos.md)-Object-Element zu erstellen, wenn das Object-Element ein direktes untergeordnetes Element des Textkörpers und für den Textkörper `data-absolute-enabled="true"` angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="963da-311">Used to create an [absolute positioned](onenote-abs-pos.md) object, only if the object is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="963da-312">Beispiel: `<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="963da-312">Example: `<object style="position:absolute;top:350px;left:300px" ... />`</span></span> |
| <span data-ttu-id="963da-313">type</span><span class="sxs-lookup"><span data-stu-id="963da-313">type</span></span> | <span data-ttu-id="963da-314">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="963da-314">Required.</span></span><br/><br/><span data-ttu-id="963da-315">Der standardmäßige Mediendateityp.</span><span class="sxs-lookup"><span data-stu-id="963da-315">The standard media file type.</span></span> <span data-ttu-id="963da-316">Bei bekannten Dateitypen wird das dem Dateityp zugeordnete Symbol auf der OneNote-Seite angezeigt.</span><span class="sxs-lookup"><span data-stu-id="963da-316">Known file types display the icon associated with the file type on the OneNote page.</span></span> <span data-ttu-id="963da-317">Bei unbekannten Dateitypen wird ein generisches Symbol angezeigt.</span><span class="sxs-lookup"><span data-stu-id="963da-317">Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

#### <a name="output-attributes"></a><span data-ttu-id="963da-318">Ausgabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-318">Output attributes</span></span>

|<span data-ttu-id="963da-319">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-319">Output attribute</span></span>|<span data-ttu-id="963da-320">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-320">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-321">data</span><span class="sxs-lookup"><span data-stu-id="963da-321">data</span></span> | <span data-ttu-id="963da-322">Der Endpunkt für die Dateiressource.</span><span class="sxs-lookup"><span data-stu-id="963da-322">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="963da-323">data-attachment</span><span class="sxs-lookup"><span data-stu-id="963da-323">data-attachment</span></span> | <span data-ttu-id="963da-324">Der Dateiname.</span><span class="sxs-lookup"><span data-stu-id="963da-324">The file name.</span></span> |
| <span data-ttu-id="963da-325">data-id</span><span class="sxs-lookup"><span data-stu-id="963da-325">data-id</span></span> | <span data-ttu-id="963da-326">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-326">A reference for the element.</span></span><br/><br/><span data-ttu-id="963da-327">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-327">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-328">id</span><span class="sxs-lookup"><span data-stu-id="963da-328">id</span></span> | <span data-ttu-id="963da-329">Eine eindeutige generierte ID für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-329">A unique, generated ID for the element.</span></span> <span data-ttu-id="963da-330">Zurückgegeben von einem [GET requests to a page's *-content*-Endpunkt ](/graph/api/page-get?view=graph-rest-1.0), wenn die `includeIDs=true`-Abfrageoption verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="963da-330">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="963da-331">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-331">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-332">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="963da-332">style</span></span> | <span data-ttu-id="963da-333">Die Positionseigenschaften des Objekts.</span><span class="sxs-lookup"><span data-stu-id="963da-333">The position properties of the object.</span></span> |
| <span data-ttu-id="963da-334">type</span><span class="sxs-lookup"><span data-stu-id="963da-334">type</span></span> | <span data-ttu-id="963da-335">Der standardmäßige Mediendateityp.</span><span class="sxs-lookup"><span data-stu-id="963da-335">The standard media file type.</span></span> |
 

#### <a name="output-html-example-for-objects"></a><span data-ttu-id="963da-336">Beispiel für Ausgabe-HTML für Objekte</span><span class="sxs-lookup"><span data-stu-id="963da-336">Output HTML example for objects</span></span>

<span data-ttu-id="963da-337">Ausgabe-**object**-Elemente enthalten Endpunkte, die wie dargestellt auf Dateiressourcen auf der Seite verweisen.</span><span class="sxs-lookup"><span data-stu-id="963da-337">Output **object** elements contain endpoints that link to the file resources in the page, as shown.</span></span> <span data-ttu-id="963da-338">Sie können separate [GET-Anforderung zu Dateiressourcen-Endpunkten](/graph/api/resource-get?view=graph-rest-1.0) durchführen, um die binäre Inhalt abzurufen.</span><span class="sxs-lookup"><span data-stu-id="963da-338">You can make separate [GET requests to file resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="963da-339">Absätze und Überschriften</span><span class="sxs-lookup"><span data-stu-id="963da-339">Paragraphs and headings</span></span>

<span data-ttu-id="963da-340">Absätze, Überschriften und andere Textcontainer können die folgenden Attribute in der Eingabe- und Ausgabe-HTML enthalten.</span><span class="sxs-lookup"><span data-stu-id="963da-340">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="963da-341">Eingabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-341">Input attributes</span></span>

|<span data-ttu-id="963da-342">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-342">Input attribute</span></span>|<span data-ttu-id="963da-343">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-343">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-344">data-id</span><span class="sxs-lookup"><span data-stu-id="963da-344">data-id</span></span> | <span data-ttu-id="963da-345">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-345">A reference for the element.</span></span><br/><br/><span data-ttu-id="963da-346">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-346">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-347">data-tag</span><span class="sxs-lookup"><span data-stu-id="963da-347">data-tag</span></span> | <span data-ttu-id="963da-348">Ein  [Notiztag ](onenote-note-tags.md) für ein **p**- oder **h1** - **h6**-Element.</span><span class="sxs-lookup"><span data-stu-id="963da-348">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="963da-349">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="963da-349">style</span></span> | <span data-ttu-id="963da-350">Die CSS-[style](#styles)-Eigenschaften des Elements.</span><span class="sxs-lookup"><span data-stu-id="963da-350">The CSS [style](#styles) properties of the element.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="963da-351">Ausgabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-351">Output attributes</span></span>

|<span data-ttu-id="963da-352">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-352">Output attribute</span></span>|<span data-ttu-id="963da-353">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-353">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-354">data-id</span><span class="sxs-lookup"><span data-stu-id="963da-354">data-id</span></span> | <span data-ttu-id="963da-355">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-355">A reference for the element.</span></span><br/><br/><span data-ttu-id="963da-356">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-356">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-357">data-tag</span><span class="sxs-lookup"><span data-stu-id="963da-357">data-tag</span></span> | <span data-ttu-id="963da-358">Ein  [Notiztag ](onenote-note-tags.md) für ein **p**- oder **h1** - **h6**-Element.</span><span class="sxs-lookup"><span data-stu-id="963da-358">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="963da-359">id</span><span class="sxs-lookup"><span data-stu-id="963da-359">id</span></span> | <span data-ttu-id="963da-360">Eine eindeutige generierte ID für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-360">A unique, generated ID for the element.</span></span> <span data-ttu-id="963da-361">Zurückgegeben von einem [GET requests to a page's *-content*-Endpunkt ](/graph/api/page-get?view=graph-rest-1.0), wenn die `includeIDs=true`-Abfrageoption verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="963da-361">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="963da-362">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-362">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-363">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="963da-363">style</span></span> | <span data-ttu-id="963da-364">Die CSS-[style](#styles)-Eigenschaften des Elements.</span><span class="sxs-lookup"><span data-stu-id="963da-364">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="963da-365">In der Ausgabe-HTML können diese Werte eingebettet in die entsprechenden untergeordneten Elemente oder in **span**-Elementen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="963da-365">In the output HTML, these values may be returned inline on appropriate child elements or on **span** elements.</span></span> |
 

<span data-ttu-id="963da-366">Die folgenden Beispiele zeigen Eingabe-HTML, die verschiedene Möglichkeiten zum Definieren von Formatvorlagen für Textcontainer verwendet, und die zurückgegebene Ausgabe-HTML.</span><span class="sxs-lookup"><span data-stu-id="963da-366">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

#### <a name="input-html-with-styles-defined-using-inline-character-styles-in-the-start-tag-and-within-a-span-element"></a><span data-ttu-id="963da-367">Eingabe-HTML, in der Formatvorlagen mit Inlinezeichenformaten, im Starttag und in einem span-Element definiert sind.</span><span class="sxs-lookup"><span data-stu-id="963da-367">Input HTML with styles defined using inline character styles, in the start tag, and within a span element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

#### <a name="output-html-with-the-i-character-style-and-the-font-settings-in-the-p-start-tag-returned-as-inline-css-styles-on-span-elements"></a><span data-ttu-id="963da-368">Ausgabe-HTML, in der das `<i>`-Zeichenformat und die Schriftarteinstellungen im `<p>`-Starttag als Inline-CSS-Formate in span-Elementen zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="963da-368">Output HTML with the `<i>` character style and the font settings in the `<p>` start tag returned as inline CSS styles on span elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="963da-369">Listen</span><span class="sxs-lookup"><span data-stu-id="963da-369">Lists</span></span>

<span data-ttu-id="963da-370">Listen werden als **ol**- oder **ul**-Elemente dargestellt, die **li**-Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="963da-370">Lists are represented as **ol** or **ul** elements that contain list items represented as **li** elements.</span></span>

<span data-ttu-id="963da-371">Listen und Listenelemente können die folgenden Attribute in der Eingabe- und Ausgabe-HTML enthalten.</span><span class="sxs-lookup"><span data-stu-id="963da-371">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="963da-372">Eingabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-372">Input attributes</span></span>

|<span data-ttu-id="963da-373">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-373">Input attribute</span></span>|<span data-ttu-id="963da-374">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-374">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-375">data-id</span><span class="sxs-lookup"><span data-stu-id="963da-375">data-id</span></span> | <span data-ttu-id="963da-376">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-376">A reference for the element.</span></span><br/><br/><span data-ttu-id="963da-377">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-377">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-378">data-tag</span><span class="sxs-lookup"><span data-stu-id="963da-378">data-tag</span></span> | <span data-ttu-id="963da-379">Ein [Notiztag](onenote-note-tags.md) für ein **ul**-, **ol**- oder **li**-Element.</span><span class="sxs-lookup"><span data-stu-id="963da-379">A [note tag](onenote-note-tags.md) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="963da-380">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="963da-380">style</span></span> | <span data-ttu-id="963da-381">Die **list-style-type**- und die CSS-[style](#styles)-Eigenschaften für die Liste oder das Listenelement.</span><span class="sxs-lookup"><span data-stu-id="963da-381">The **list-style-type** and the CSS [style](#styles) properties for the list or list item.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="963da-382">Ausgabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-382">Output attributes</span></span>

|<span data-ttu-id="963da-383">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-383">Output attribute</span></span>|<span data-ttu-id="963da-384">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-384">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-385">data-id</span><span class="sxs-lookup"><span data-stu-id="963da-385">data-id</span></span> | <span data-ttu-id="963da-386">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-386">A reference for the element.</span></span><br/><br/><span data-ttu-id="963da-387">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-387">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-388">data-tag</span><span class="sxs-lookup"><span data-stu-id="963da-388">data-tag</span></span> |  <span data-ttu-id="963da-389">Ein [Notiztag](onenote-note-tags.md) für ein span-Objekt in einem **li**-Element.</span><span class="sxs-lookup"><span data-stu-id="963da-389">A [note tag](onenote-note-tags.md) on a span in an **li** element.</span></span> |
| <span data-ttu-id="963da-390">id</span><span class="sxs-lookup"><span data-stu-id="963da-390">id</span></span> | <span data-ttu-id="963da-391">Eine eindeutige generierte ID für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-391">A unique, generated ID for the element.</span></span> <span data-ttu-id="963da-392">Zurückgegeben von einem [GET requests to a page's *-content*-Endpunkt ](/graph/api/page-get?view=graph-rest-1.0), wenn die `includeIDs=true`-Abfrageoption verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="963da-392">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="963da-393">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-393">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-394">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="963da-394">style</span></span> | <span data-ttu-id="963da-395">Die **list-style-type**- und CSS-[style](#styles)-Eigenschaften des Elements.</span><span class="sxs-lookup"><span data-stu-id="963da-395">The **list-style-type** and CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="963da-396">In der Ausgabe HTML werden die Listenebene-Einstellungen an die  Listenelemente zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="963da-396">In the output HTML, list-level settings are returned on list items.</span></span> <span data-ttu-id="963da-397">Standard-Eigenschaften werden nicht zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="963da-397">Default properties are not returned.</span></span> |
 
### <a name="list-styles"></a><span data-ttu-id="963da-398">Listenformatvorlagen</span><span class="sxs-lookup"><span data-stu-id="963da-398">List styles</span></span>

<span data-ttu-id="963da-399">Die OneNote-APIs in Microsoft Graph unterstützen die folgenden Listentypen:</span><span class="sxs-lookup"><span data-stu-id="963da-399">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="963da-400">Sortierte Liste</span><span class="sxs-lookup"><span data-stu-id="963da-400">Ordered list</span></span>|<span data-ttu-id="963da-401">Unsortierte Liste</span><span class="sxs-lookup"><span data-stu-id="963da-401">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="963da-402">keine</span><span class="sxs-lookup"><span data-stu-id="963da-402">none</span></span> | <span data-ttu-id="963da-403">Keine</span><span class="sxs-lookup"><span data-stu-id="963da-403">none</span></span> |
| <span data-ttu-id="963da-404">
decimal (Standard)</span><span class="sxs-lookup"><span data-stu-id="963da-404">decimal (default)</span></span> | <span data-ttu-id="963da-405">
disc (Standard)</span><span class="sxs-lookup"><span data-stu-id="963da-405">disc (default)</span></span> |
| <span data-ttu-id="963da-406">lower-alpha</span><span class="sxs-lookup"><span data-stu-id="963da-406">lower-alpha</span></span> | <span data-ttu-id="963da-407">circle</span><span class="sxs-lookup"><span data-stu-id="963da-407">circle</span></span> |
| <span data-ttu-id="963da-408">lower-roman</span><span class="sxs-lookup"><span data-stu-id="963da-408">lower-roman</span></span> | <span data-ttu-id="963da-409">

square</span><span class="sxs-lookup"><span data-stu-id="963da-409">square</span></span> |
| <span data-ttu-id="963da-410">
upper-alpha</span><span class="sxs-lookup"><span data-stu-id="963da-410">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="963da-411">upper-roman</span><span class="sxs-lookup"><span data-stu-id="963da-411">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="963da-412">Sie können globale Formatvorlagen für eine Liste im **ol**- oder **ul**-Element in der Eingabe-HTML anwenden, aber Formatvorlagen werden in den **li**-Elementen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="963da-412">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

#### <a name="homogenous-list-style"></a><span data-ttu-id="963da-413">Homogene Listenformatvorlage</span><span class="sxs-lookup"><span data-stu-id="963da-413">Homogenous list style</span></span>

<span data-ttu-id="963da-414">Dieses Beispiel zeigt Eingabe-HTML, die den Listenformattyp im **ol**-Element und CSS-Formatvorlagen in einzelnen Listenelementen festlegt.</span><span class="sxs-lookup"><span data-stu-id="963da-414">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="963da-p138">Dies ist die Ausgabe-HTML. Beachten Sie, dass Formatvorlagen inline in den einzelnen **li**- oder **span**-Elementen zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="963da-p138">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

#### <a name="variable-list-styles"></a><span data-ttu-id="963da-417">Variable Listenelementvorlagen</span><span class="sxs-lookup"><span data-stu-id="963da-417">Variable list styles</span></span>

<span data-ttu-id="963da-418">Dieses Beispiel zeigt Eingabe-HTML, die verschiedene Listenformattypen in den **li**-Elementen festlegt.</span><span class="sxs-lookup"><span data-stu-id="963da-418">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="963da-p139">Dies ist die Ausgabe-HTML. Beachten Sie, dass Formatvorlagen inline in den einzelnen **li**- oder **span**-Elementen zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="963da-p139">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="963da-421">Tabellen</span><span class="sxs-lookup"><span data-stu-id="963da-421">Tables</span></span>

<span data-ttu-id="963da-p140">Tabellen werden als **table**-Elemente dargestellt, die **tr**- und **td**-Elemente enthalten können. Geschachtelte Tabellen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="963da-p140">Tables are represented as **table** elements that can contain **tr** and **td** elements. Nested tables are supported.</span></span>

<span data-ttu-id="963da-424">Tabellen können die folgenden Attribute in der Eingabe- und Ausgabe-HTML enthalten.</span><span class="sxs-lookup"><span data-stu-id="963da-424">Tables can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="963da-425">Die OneNote-APIs unterstützen keine **rowspan**- oder **colspan**-Attribute.</span><span class="sxs-lookup"><span data-stu-id="963da-425">The OneNote APIs do not support **rowspan** or **colspan** attributes.</span></span> 

#### <a name="input-attributes"></a><span data-ttu-id="963da-426">Eingabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-426">Input attributes</span></span>

|<span data-ttu-id="963da-427">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-427">Input attribute</span></span>|<span data-ttu-id="963da-428">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-428">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-429">data-id</span><span class="sxs-lookup"><span data-stu-id="963da-429">data-id</span></span> | <span data-ttu-id="963da-430">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-430">A reference for the element.</span></span><br/><br/><span data-ttu-id="963da-431">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-431">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-432">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="963da-432">style</span></span> | <span data-ttu-id="963da-433">Die CSS-[style](#styles)-Eigenschaften des Elements und:</span><span class="sxs-lookup"><span data-stu-id="963da-433">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="963da-434">- **border**.</span><span class="sxs-lookup"><span data-stu-id="963da-434">- **border**.</span></span> <span data-ttu-id="963da-435">Kann entweder 0px oder 1px sein.</span><span class="sxs-lookup"><span data-stu-id="963da-435">Can be either 0px or 1px.</span></span><br/> <span data-ttu-id="963da-436">- **width**.</span><span class="sxs-lookup"><span data-stu-id="963da-436">- **width**.</span></span> <span data-ttu-id="963da-437">**width**. Unterstützt von **table** und td als Pixel oder Prozentsatz der Seitenbreite.</span><span class="sxs-lookup"><span data-stu-id="963da-437">Supported by **table** and **td** as pixels or percentage of page width.</span></span><br/><br/><span data-ttu-id="963da-438">Beispiele: `width="100px"` oder `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="963da-438">Example: `width="100px"` or `width="60%"`</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="963da-439">Ausgabeattribute</span><span class="sxs-lookup"><span data-stu-id="963da-439">Output attributes</span></span>

|<span data-ttu-id="963da-440">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="963da-440">Output attribute</span></span>|<span data-ttu-id="963da-441">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="963da-441">Description</span></span>|
|:------|:------|
| <span data-ttu-id="963da-442">data-id</span><span class="sxs-lookup"><span data-stu-id="963da-442">data-id</span></span> | <span data-ttu-id="963da-443">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-443">A reference for the element.</span></span><br/><br/><span data-ttu-id="963da-444">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-444">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-445">id</span><span class="sxs-lookup"><span data-stu-id="963da-445">id</span></span> | <span data-ttu-id="963da-446">Eine eindeutige generierte ID für das Element.</span><span class="sxs-lookup"><span data-stu-id="963da-446">A unique, generated ID for the element.</span></span> <span data-ttu-id="963da-447">Zurückgegeben von einem [GET requests to a page's *-content*-Endpunkt ](/graph/api/page-get?view=graph-rest-1.0), wenn die `includeIDs=true`-Abfrageoption verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="963da-447">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="963da-448">Wird verwendet, um [Seiteninhalt zu aktualisieren](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="963da-448">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="963da-449">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="963da-449">style</span></span> | <span data-ttu-id="963da-450">Die CSS-[style](#styles)-Eigenschaften des Elements.</span><span class="sxs-lookup"><span data-stu-id="963da-450">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="963da-451">Die folgenden Beispiele zeigen Eingabe-HTML, die verschiedene Möglichkeiten zum Definieren von Formatvorlagen für Tabellen verwendet, und die zurückgegebene Ausgabe-HTML.</span><span class="sxs-lookup"><span data-stu-id="963da-451">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

#### <a name="input-html-with-optional-settings-at-different-levels"></a><span data-ttu-id="963da-452">Eingabe HTML mit optionalen Einstellungen auf verschiedenen Ebenen</span><span class="sxs-lookup"><span data-stu-id="963da-452">Input HTML with optional settings at different levels</span></span>

```html
<table style="border:0px;width:500px;background-color:green">
    <tr> 
        <td>Cell 1</td> 
        <td>Cell 2</td> 
        <td>Cell 3</td> 
    </tr> 
    <tr style="background-color:blue"> 
        <td style="text-align:right;background-color:red">Left</td> 
        <td style="text-align:center">Middle</td> 
        <td>Right</td> 
    </tr> 
</table>
```
 
#### <a name="output-html-with-css-styles-returned-inline-on-the-td-elements"></a><span data-ttu-id="963da-453">Ausgabe-HTML mit inline in td-Elementen zurückgegebenen CSS-Formatvorlagen</span><span class="sxs-lookup"><span data-stu-id="963da-453">Output HTML with CSS styles returned inline on the td elements</span></span>

```html
<table style="border:0px">
    <tr>
        <td style="background-color:green;width:166;border:0px">Cell 1</td>
        <td style="background-color:green;width:166;border:0px">Cell 2</td>
        <td style="background-color:green;width:166;border:0px">Cell 3</td>
    </tr>
    <tr>
        <td style="background-color:red;width:166;border:0px;text-align:right">Left</td>
        <td style="background-color:blue;width:166;border:0px;text-align:center">Middle</td>
        <td style="background-color:blue;width:166;border:0px">Right</td>
    </tr>
</table>
``` 


## <a name="styles"></a><span data-ttu-id="963da-454">Formatvorlagen</span><span class="sxs-lookup"><span data-stu-id="963da-454">Styles</span></span>

<span data-ttu-id="963da-455">OneNote APIs in Microsoft Graph unterstützt die folgenden Inline-CSS-**style**-Eigenschaften für Elemente im Seitentextkörper, wie **body**, **div**, **p**, **li** und **span**.</span><span class="sxs-lookup"><span data-stu-id="963da-455">OneNote APIs in Microsoft Graph support the following inline CSS **style** properties for elements in the page body, such as **body**, **div**, **p**, **li**, and **span**.</span></span>

|<span data-ttu-id="963da-456">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="963da-456">Property</span></span>|<span data-ttu-id="963da-457">Beispiel</span><span class="sxs-lookup"><span data-stu-id="963da-457">Example</span></span>|
|:------|:------|
| <span data-ttu-id="963da-458">background-color</span><span class="sxs-lookup"><span data-stu-id="963da-458">background-color</span></span> | <span data-ttu-id="963da-459">`style="background-color:#66cc66"` (Standardwert ist Weiß)</span><span class="sxs-lookup"><span data-stu-id="963da-459">`style="background-color:#66cc66"` (defaults to white)</span></span><br/><br/><span data-ttu-id="963da-460">Das hexadezimale Format und benannte Farben werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="963da-460">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="963da-461">color</span><span class="sxs-lookup"><span data-stu-id="963da-461">color</span></span> | <span data-ttu-id="963da-462">`style="color:#ffffff"` (Standardwert ist Schwarz)</span><span class="sxs-lookup"><span data-stu-id="963da-462">`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="963da-463">font-family</span><span class="sxs-lookup"><span data-stu-id="963da-463">font-family</span></span> | <span data-ttu-id="963da-464">`style="font-family:Courier"` (Standardwert ist Calibri)</span><span class="sxs-lookup"><span data-stu-id="963da-464">`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="963da-465">font-size</span><span class="sxs-lookup"><span data-stu-id="963da-465">font-size</span></span> | <span data-ttu-id="963da-466">`style="font-size:10pt"` (Standardwert ist 11pt)</span><span class="sxs-lookup"><span data-stu-id="963da-466">`style="font-size:10pt"` (defaults to 11pt)</span></span><br/><br/><span data-ttu-id="963da-467">Die APIs akzeptieren den Schriftgrad in *pt* oder *px*, *px* wird jedoch zu *pt* konvertiert.</span><span class="sxs-lookup"><span data-stu-id="963da-467">The APIs accept font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="963da-468">Dezimalwerte werden auf die nächste n.0pt oder n.5pt gerundet.</span><span class="sxs-lookup"><span data-stu-id="963da-468">Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="963da-469">font-style</span><span class="sxs-lookup"><span data-stu-id="963da-469">font-style</span></span> | <span data-ttu-id="963da-470">`style="font-style:italic"`(nur normal oder kursiv)</span><span class="sxs-lookup"><span data-stu-id="963da-470">`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="963da-471">font-weight</span><span class="sxs-lookup"><span data-stu-id="963da-471">font-weight</span></span> | <span data-ttu-id="963da-472">`style="font-weight:bold"`(nur normal oder fett)</span><span class="sxs-lookup"><span data-stu-id="963da-472">`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="963da-473">strike-through</span><span class="sxs-lookup"><span data-stu-id="963da-473">strike-through</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="963da-474">text-align</span><span class="sxs-lookup"><span data-stu-id="963da-474">text-align</span></span> | <span data-ttu-id="963da-475">`style="text-align:center"`(nur für Blockelementen)</span><span class="sxs-lookup"><span data-stu-id="963da-475">`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="963da-476">text-decoration</span><span class="sxs-lookup"><span data-stu-id="963da-476">text-decoration</span></span> | <span data-ttu-id="963da-477">`style="text-decoration:underline"`(nur keine oder unterstrichen)</span><span class="sxs-lookup"><span data-stu-id="963da-477">`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="963da-478">Die folgenden Inlinezeichenformate werden ebenfalls unterstützt:</span><span class="sxs-lookup"><span data-stu-id="963da-478">The following inline character styles are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="963da-479"><b></span><span class="sxs-lookup"><span data-stu-id="963da-479"><b></span></span></td>
<td id="simplecell"><span data-ttu-id="963da-480"><i></span><span class="sxs-lookup"><span data-stu-id="963da-480"><i></span></span></td>
<td id="simplecell"><span data-ttu-id="963da-481"><u></span><span class="sxs-lookup"><span data-stu-id="963da-481"><u></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="963da-482"><em></span><span class="sxs-lookup"><span data-stu-id="963da-482"><em></span></span></td>
<td id="simplecell"><span data-ttu-id="963da-483"><strong></span><span class="sxs-lookup"><span data-stu-id="963da-483"><strong></span></span></td>
<td id="simplecell"><span data-ttu-id="963da-484"><strike></span><span class="sxs-lookup"><span data-stu-id="963da-484"><strike></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="963da-485"><sup></span><span class="sxs-lookup"><span data-stu-id="963da-485"><sup></span></span></td>
<td id="simplecell"><span data-ttu-id="963da-486"><sub></span><span class="sxs-lookup"><span data-stu-id="963da-486"><sub></span></span></td>
<td id="simplecell"><span data-ttu-id="963da-487"><del></span><span class="sxs-lookup"><span data-stu-id="963da-487"><del></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="963da-488"><cite></span><span class="sxs-lookup"><span data-stu-id="963da-488"><cite></span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="963da-489">Beispiel für Eingabe- und Ausgabe-HTML</span><span class="sxs-lookup"><span data-stu-id="963da-489">Input and output HTML example</span></span>

<span data-ttu-id="963da-490">Die folgende Abbildung zeigt eine einfache Seite, die mit der Microsoft Graph erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="963da-490">The following image shows a simple page that was created with Microsoft Graph.</span></span>

![Bild einer OneNote-Seite mit Lernnotizen aus Inhalten von Wikipedia](images/onenote-sample-image.png)

<span data-ttu-id="963da-492">Dabei handelt es sich um die Eingabe-HTML, die im Nachrichtentextkörper gesendet wurde, um die Seite zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="963da-492">This is the input HTML sent in the message body to create the page.</span></span>

```html
<html lang="en-US">
    <head>
        <title>Sample Study Notes</title>
        <meta name="created" content="2015-01-01T01:01"/>
    </head>
    <body>
        <h1>Aurora Borealis</h1>
        <p>Dancing lights in the sky. Also called <i>Northern Lights</i>. Caused by solar radiation.</p>
        <br />
        <p><b>Intersting facts</b></p>
        <table>
            <tr>
                <td>Neil Armstrong</td>
                <td>Commander</td>
            </tr>
            <tr>
                <td>Buzz Aldrin</td>
                <td>LM Pilot</td>
            </tr>
            <tr>
                <td>Michael Collins</td>
                <td>Command Module Pilot</td>
            </tr>
        </table>
        <img alt="Apollo 11 commemorative stamp." src="https://upload.wikimedia.org/wikipedia/commons/a/a4/First_Man_on_Moon_1969_Issue-10c.jpg"  width="400"/>
        <p>References:</p>
        <p><a href="https://en.wikipedia.org/wiki/Apollo_11">https://en.wikipedia.org/wiki/Apollo_11</a></p>
        <p><a href="https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
    </body>
</html>
``` 

<br/>

<span data-ttu-id="963da-493">Im Folgenden sehen Sie die Ausgabe-HTML, die die Microsoft Graph zurückgibt, wenn Sie [den Seiteninhalt abrufen](onenote-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="963da-493">This is the output HTML that Microsoft Graph returns when you [get page content](onenote-get-content.md).</span></span>

> <span data-ttu-id="963da-494">**Hinweis:** Wenn Sie [eine Seite erstellen](onenote-create-page.md) oder [die Metadaten einer Seite abrufen](/graph/api/page-get?view=graph-rest-1.0), gibt die API die *Inhalte*-Endpunkt-URL der Seite in der **contentUrl**Eigenschaft zurück.</span><span class="sxs-lookup"><span data-stu-id="963da-494">**Note:** When you [create a page](onenote-create-page.md) or [get page metadata](/graph/api/page-get?view=graph-rest-1.0), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

```html
<html htmlns="https://www.w3.org/1999/xhtml" lang="en-US">
    <head>
        <title>Sample Study Notes</title>
    </head>
    <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11pt">
        <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
            <h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">American History 101: Moon Landing</h1>
            <p>First moon landing - July 20, 1969 with Apollo 11 (Eagle)</p>
            <br />
            <p><span style="font-weight:bold">Apollo 11 Astronauts</span></p>
            <table style="border:0px">
                <tr>
                    <td style="border:0px">Neil Armstrong</td>
                    <td style="border:0px">Commander</td>
                </tr>
                <tr>
                    <td style="border:0px">Buzz Aldrin</td>
                    <td style="border:0px">LM Pilot</td>
                </tr>
                <tr>
                    <td style="border:0px">Michael Collins</td>
                    <td style="border:0px">Command Module Pilot</td>
                </tr>
            </table>
            <br />
            <img alt="Apollo 11 commemorative stamp." width="400" height="248" src="https://graph.microsoft.com/v1.0/me/onenote/resources/0-f717b5fa5eaa454da7ecdf72a8c137fe!1-73DBAF9B7E5C4B4C!10456/$value"
                 data-src-type="image/jpeg" data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/0-f717b5fa5eaa454da7ecdf72a8c137fe!1-73DBAF9B7E5C4B4C!10456/$value" data-fullres-src-type="image/jpeg" />
            <p>References:</p>
            <p><a href="https://en.wikipedia.org/wiki/Apollo_11">https://en.wikipedia.org/wiki/Apollo_11</a></p>
            <p><a href="https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
        </div>
    </body>
</html>
``` 

## <a name="see-also"></a><span data-ttu-id="963da-495">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="963da-495">See also</span></span>

- [<span data-ttu-id="963da-496">Abrufen von OneNote-Inhalt und -Struktur</span><span class="sxs-lookup"><span data-stu-id="963da-496">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="963da-497">Erstellen von OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="963da-497">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="963da-498">Aktualisieren der Inhalte von OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="963da-498">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="963da-499">Hinzufügen von Bildern, Videos und Dateien</span><span class="sxs-lookup"><span data-stu-id="963da-499">Add images, videos, and files</span></span>](onenote-images-files.md)
