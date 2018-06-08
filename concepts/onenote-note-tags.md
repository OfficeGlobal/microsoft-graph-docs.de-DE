# <a name="use-note-tags-in-onenote-pages"></a><span data-ttu-id="90932-101">Verwenden von Notiztags auf OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="90932-101">Use note tags in OneNote pages</span></span>

<span data-ttu-id="90932-102">*__Gilt für:__ Privatanwender-Notizbücher auf OneDrive | Enterprise-Notizbücher auf Office 365*</span><span class="sxs-lookup"><span data-stu-id="90932-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>

<span data-ttu-id="90932-103">Verwenden Sie das `data-tag`-Attribut zum Hinzufügen und Aktualisieren von Kontrollkästchen, Sternen und anderen integrierten Notiztags auf einer OneNote-Seite, wie in der folgenden Abbildung gezeigt.</span><span class="sxs-lookup"><span data-stu-id="90932-103">Use the `data-tag` attribute to add and update check boxes, stars, and other built-in note tags on a OneNote page, as shown in the following image.</span></span>

![Drei Notiztags auf einer OneNote-Seite.](images/note-tags-example.PNG)


<a name="attributes"></a>
## <a name="note-tag-attributes"></a><span data-ttu-id="90932-105">Notiztag-Attribute</span><span class="sxs-lookup"><span data-stu-id="90932-105">Note tag attributes</span></span>

<span data-ttu-id="90932-106">Ein Notiztag wird im HTML-Code einer OneNote-Seite durch das `data-tag`-Attribut dargestellt.</span><span class="sxs-lookup"><span data-stu-id="90932-106">In the HTML of a onnvshort page, a note tag is represented by the data-tag attribute. For example:</span></span> <span data-ttu-id="90932-107">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="90932-107">For example:</span></span>

- <span data-ttu-id="90932-108">Ein deaktiviertes Aufgabenfeld:  `<p data-tag="to-do">`</span><span class="sxs-lookup"><span data-stu-id="90932-108">An unchecked to-do box:  <p data-tag="to-do">`<p data-tag="to-do">`</span></span> 
- <span data-ttu-id="90932-109">Ein aktiviertes Aufgabenfeld:  `<p data-tag="to-do:completed">`</span><span class="sxs-lookup"><span data-stu-id="90932-109">A checked to-do box:  <p data-tag="to-do:completed">`<p data-tag="to-do:completed">`</span></span> 
- <span data-ttu-id="90932-110">Ein Stern:  `<h2 data-tag="important">`</span><span class="sxs-lookup"><span data-stu-id="90932-110">A star:  `<h2 data-tag="important">`</span></span> 

<span data-ttu-id="90932-111">Ein `data-tag`-Wert besteht aus einem Shape und manchmal einem Status.</span><span class="sxs-lookup"><span data-stu-id="90932-111">A `data-tag` value is composed of a shape, and sometimes a status.</span></span> <span data-ttu-id="90932-112">(*siehe [unterstützte Werte](#built-in-note-tags-for-onenote)*)</span><span class="sxs-lookup"><span data-stu-id="90932-112">(*see all [supported values](#built-in-note-tags-for-onenote)*)</span></span>

| <span data-ttu-id="90932-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="90932-113">Property</span></span> | <span data-ttu-id="90932-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90932-114">Description</span></span> |  
|:------|:------|  
| <span data-ttu-id="90932-115">shape</span><span class="sxs-lookup"><span data-stu-id="90932-115">shape</span></span> | <span data-ttu-id="90932-116">Der Bezeichner für das Notiztag (Beispiel: `to-do` oder `important`).</span><span class="sxs-lookup"><span data-stu-id="90932-116">The identifier of the note tag (example: to-do`to-do` or important`important`).</span></span> |  
| <span data-ttu-id="90932-117">status</span><span class="sxs-lookup"><span data-stu-id="90932-117">status</span></span> | <span data-ttu-id="90932-118">Der Status der Kontrollkästchen von Notiztags.</span><span class="sxs-lookup"><span data-stu-id="90932-118">The status of check-box note tags.</span></span> <span data-ttu-id="90932-119">Dies wird nur dazu verwendet, die Kontrollkästchen als abgeschlossen zu kennzeichnen.</span><span class="sxs-lookup"><span data-stu-id="90932-119">The status of check-box note tags. This is used only to set check boxes as  completed.</span></span> |  
 

<a name="note-tags"></a>
## <a name="add-or-update-note-tags"></a><span data-ttu-id="90932-120">Hinzufügen oder Aktualisieren von Notiztags</span><span class="sxs-lookup"><span data-stu-id="90932-120">Add or update note tags on onnvshort pages</span></span>

<span data-ttu-id="90932-121">Verwenden Sie zum Hinzufügen oder Aktualisieren eines integrierten Notiztags das `data-tag`-Attribut für ein unterstütztes Element.</span><span class="sxs-lookup"><span data-stu-id="90932-121">To add or update a built-in note tag, just use the `data-tag` attribute on a supported element.</span></span> <span data-ttu-id="90932-122">Im Folgenden ist z. B. ein Absatz als wichtig gekennzeichnet:</span><span class="sxs-lookup"><span data-stu-id="90932-122">For example, here's a paragraph marked as important:</span></span>

```html
<p data-tag="important">...</p>
```

<span data-ttu-id="90932-123">Trennen Sie mehrere Notiztags durch Kommas:</span><span class="sxs-lookup"><span data-stu-id="90932-123">Separate multiple note tags with commas:</span></span>

```html
<p data-tag="important, critical">...</p>
```

<span data-ttu-id="90932-124">Sie können ein `data-tag` für die folgenden Elemente definieren:</span><span class="sxs-lookup"><span data-stu-id="90932-124">You can define the data-tag attribute on  the following elements:</span></span>

- <span data-ttu-id="90932-125">p</span><span class="sxs-lookup"><span data-stu-id="90932-125">p</span></span> 
- <span data-ttu-id="90932-126">ul, ol, li (*Weitere Informationen zu [Notiztags in Listen](#note-tags-on-lists)*)</span><span class="sxs-lookup"><span data-stu-id="90932-126">ul, ol, li (see more about lists)</span></span>
- <span data-ttu-id="90932-127">img</span><span class="sxs-lookup"><span data-stu-id="90932-127">img</span></span> 
- <span data-ttu-id="90932-128">h1 – h6</span><span class="sxs-lookup"><span data-stu-id="90932-128">h1 - h6</span></span> 
- <span data-ttu-id="90932-129">title</span><span class="sxs-lookup"><span data-stu-id="90932-129">title</span></span> 

<span data-ttu-id="90932-130">Eine Liste der Notiztags, die Sie mit Microsoft Graph verwenden können, finden Sie unter [Integrierte Notiztags](#built-in-note-tags-for-onenote).</span><span class="sxs-lookup"><span data-stu-id="90932-130">See Built-in note tags for OneNote for a list of note tags that you can use with the onnvshort API.</span></span> <span data-ttu-id="90932-131">Das Hinzufügen oder Aktualisieren von benutzerdefinierten Tags mit Microsoft Graph wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="90932-131">Adding or updating custom tags using the onnvshort API is not supported.</span></span>
 
<span data-ttu-id="90932-132">**Beispiele**</span><span class="sxs-lookup"><span data-stu-id="90932-132">**Examples**</span></span>

<span data-ttu-id="90932-133">Im Folgenden finden Sie eine einfache Aufgabenliste, in der das erste Element abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="90932-133">Here's a simple to-do list with the first item completed.</span></span>

```html 
<p data-tag="to-do:completed" data-id="prep">Till garden bed</p> 
<p data-tag="to-do" data-id="spring">Plant peas and spinach</p>
<p data-tag="to-do" data-id="summer">Plant tomatoes and peppers</p>
```

<span data-ttu-id="90932-134">Beachten Sie, dass die oben aufgeführten `<p>`-Tags jeweils ein `data-id`-Attribut enthalten.</span><span class="sxs-lookup"><span data-stu-id="90932-134">Note that the `<p>` tags above each include a `data-id` attribute.</span></span> <span data-ttu-id="90932-135">Auf diese Weise ist es einfacher, die Kontrollkästchen für Notiztags zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="90932-135">This makes it easier to update the check-box note tags.</span></span> <span data-ttu-id="90932-136">Mit der folgenden Anforderung wird z. B. die spring-Aufgabe Pflanzen als abgeschlossen gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="90932-136">For example, the following request marks the spring planting to-do item as completed.</span></span>

``` 
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#spring',
    'action':'replace',
    'content':'<p data-tag="to-do:completed"  data-id="spring">Plant peas and spinach</p>'
  }
]
```

<span data-ttu-id="90932-137">Die folgende Anforderung erstellt eine Seite, die alle [integrierten Notiztags](#built-in-note-tags-for-onenote) enthält.</span><span class="sxs-lookup"><span data-stu-id="90932-137">The following request creates a page that contains all built-in note tags.</span></span>

``` 
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages

Content-Type: text/html
Authorization: Bearer {token}


<!DOCTYPE html>
<html>
  <head>
    <title data-tag="to-do:completed">All built-in note tags</title>
  </head>
  <body>
    <h1 data-tag="important">Paragraphs with built-in note tags</h1>
    <p data-tag="to-do">to-do</p>
    <p data-tag="important">important</p>
    <p data-tag="question">question</p>
    <p data-tag="definition">definition</p>
    <p data-tag="highlight">highlight</p>
    <p data-tag="contact">contact</p>
    <p data-tag="address">address</p>
    <p data-tag="phone-number">phone-number</p>
    <p data-tag="web-site-to-visit">web-site-to-visit</p>
    <p data-tag="idea">idea</p>
    <p data-tag="password">password</p>
    <p data-tag="critical">critical</p>
    <p data-tag="project-a">project-a</p>
    <p data-tag="project-b">project-b</p>
    <p data-tag="remember-for-later">remember-for-later</p>
    <p data-tag="movie-to-see">movie-to-see</p>
    <p data-tag="book-to-read">book-to-read</p>
    <p data-tag="music-to-listen-to">music-to-listen-to</p>
    <p data-tag="source-for-article">source-for-article</p>
    <p data-tag="remember-for-blog">remember-for-blog</p>
    <p data-tag="discuss-with-person-a">discuss-with-person-a</p>
    <p data-tag="discuss-with-person-b">discuss-with-person-b</p>
    <p data-tag="discuss-with-manager">discuss-with-manager</p>
    <p data-tag="send-in-email">send-in-email</p>
    <p data-tag="schedule-meeting">schedule-meeting</p>
    <p data-tag="call-back">call-back</p>
    <p data-tag="to-do-priority-1">to-do-priority-1</p>
    <p data-tag="to-do-priority-2">to-do-priority-2</p>
    <p data-tag="client-request">client-request</p>
    <h1 data-tag="important">Paragraphs with check boxes marked with "completed" status</h1>
    <p data-tag="to-do:completed">to-do:completed</p>
    <p data-tag="discuss-with-person-a:completed">discuss-with-person-a:completed</p>
    <p data-tag="discuss-with-person-b:completed">discuss-with-person-b:completed</p>
    <p data-tag="discuss-with-manager:completed">discuss-with-manager:completed</p>
    <p data-tag="schedule-meeting:completed">schedule-meeting:completed</p>
    <p data-tag="call-back:completed">call-back:completed</p>
    <p data-tag="to-do-priority-1:completed">to-do-priority-1:completed</p>
    <p data-tag="to-do-priority-2:completed">to-do-priority-2:completed</p>
    <p data-tag="client-request:completed">client-request:completed</p>
    <h1 data-tag="important">Multiple note tags</h1>
    <p data-tag="project-a,  client-request:completed">Two note tags:  project-a, client-request:completed</p>
    <p data-tag="idea, send-in-email, question">Three note tags:  idea, send-in-email, question</p>
    <h1 data-tag="important">Using note tags with other elements</h1>
    <p><b>Note tag on a list item:</b></p>
    <ul>
      <li data-tag="to-do-priority-1:completed">Make a to-do list</li>
    </ul>
    <p><b>Note tag on an image:</b></p>
    <img data-tag="source-for-article" src="http://placecorgi.com/200" />
    <p><b>Note tag with embedded style:</b></p>
    <p data-tag="important">Next time, <b>don't</b> forget to invite <span style="background-color:yellow">Dan</span>.</p>
  </body>
</html>
``` 

<span data-ttu-id="90932-138">Weitere Informationen zum Erstellen von Seiten finden Sie unter [Erstellen von OneNote-Seiten](onenote-create-page.md).</span><span class="sxs-lookup"><span data-stu-id="90932-138">For more information about creating pages, see [Create OneNote pages](onenote-create-page.md).</span></span> <span data-ttu-id="90932-139">Weitere Informationen zum Aktualisieren von Seiten finden Sie unter [Aktualisieren von OneNote-Seiten](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="90932-139">For more about updating pages, see [Update OneNote pages](onenote_update_page.md).</span></span>


<a name="note-tags-lists"></a>
### <a name="note-tags-on-lists"></a><span data-ttu-id="90932-140">Notiztags in Listen</span><span class="sxs-lookup"><span data-stu-id="90932-140">Note tags on lists</span></span>

<span data-ttu-id="90932-141">Hier sind einige Richtlinien für das Arbeiten mit Notiztags in Listen:</span><span class="sxs-lookup"><span data-stu-id="90932-141">Here are some guidelines for working with note tags on lists:</span></span>

- <span data-ttu-id="90932-142">Verwenden Sie `p`-Elemente für Aufgabenlisten.</span><span class="sxs-lookup"><span data-stu-id="90932-142">Use `p` elements for to-do lists.</span></span> <span data-ttu-id="90932-143">Sie zeigen keine Aufzählungen oder Nummern an und können einfacher aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="90932-143">Use p elements for to-do lists. They don't display a bullet or number, and they're easier to update.</span></span>

- <span data-ttu-id="90932-144">So erstellen oder aktualisieren Sie Listen, die das **gleiche** Notiztag für alle Listenelemente anzeigen:</span><span class="sxs-lookup"><span data-stu-id="90932-144">To create or update ul or ol elements that display the **same**  note tag for all list items:</span></span>
  
   <p id="indent"><span data-ttu-id="90932-145">Definieren Sie `data-tag` für `ul` oder `ol`.</span><span class="sxs-lookup"><span data-stu-id="90932-145">Define `data-tag` on the `ul` or `ol`.</span></span> <span data-ttu-id="90932-146">Um die gesamte Liste zu aktualisieren, müssen Sie `data-tag` für `ul` oder `ol` neu definieren.</span><span class="sxs-lookup"><span data-stu-id="90932-146">Define data-tag`data-tag` on the ul`ul` or ol`ol`. To update the entire list, you'll need to redefine  data-tag on the ul or ol.</span></span></p>

- <span data-ttu-id="90932-147">So erstellen oder aktualisieren Sie Listen, die ein **eindeutiges** Notiztag für einige oder alle Elemente anzeigen:</span><span class="sxs-lookup"><span data-stu-id="90932-147">To create or update ul or ol elements that display the **same**  note tag for all list items:</span></span>
  
   <p id="indent"><span data-ttu-id="90932-148">Definieren Sie `data-tag` für `li`-Elemente, und schachteln Sie die `li`-Elemente nicht in einem `ul`- oder `ol`-Element.</span><span class="sxs-lookup"><span data-stu-id="90932-148">Define `data-tag` on `li` elements, and don't nest the `li` elements in a `ul` or `ol`.</span></span> <span data-ttu-id="90932-149">Um die gesamte Liste zu aktualisieren, müssen Sie das `ul`-Element, das in der HTML-Ausgabe zurückgegeben wird, entfernen und nur die ungeschachtelten `li`-Elemente zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="90932-149">To update the entire list, you'll need to remove the `ul` that's returned in the output HTML and provide only the unnested `li` elements.</span></span></p>

- <span data-ttu-id="90932-150">So aktualisieren Sie bestimmte `li` Elemente:</span><span class="sxs-lookup"><span data-stu-id="90932-150">To update specific li`li` elements:</span></span>

   <p id="indent"><span data-ttu-id="90932-151">Wählen Sie die `li`-Elemente einzeln aus, und definieren Sie das `data-tag` für das `li`-Element.</span><span class="sxs-lookup"><span data-stu-id="90932-151">Target the `li` elements individually and define the `data-tag` on the `li` element.</span></span> <span data-ttu-id="90932-152">Ein einzeln adressiertes `li`-Element kann so aktualisiert werden, dass es ein eindeutiges Notiztag anzeigt, unabhängig davon, wie die Liste ursprünglich definiert wurde.</span><span class="sxs-lookup"><span data-stu-id="90932-152">Any individually addressed `li` element can be updated to display a unique note tag, no matter how the list was originally defined.</span></span></p>

<span data-ttu-id="90932-153">Die Richtlinien basieren auf den folgenden Regeln, die von Microsoft Graph angewendet werden:</span><span class="sxs-lookup"><span data-stu-id="90932-153">The guidelines are based on the following rules that are applied by Microsoft Graph:</span></span>

- <span data-ttu-id="90932-154">Die `data-tag`-Einstellung für ein `ul`- oder `ol`-Element überschreibt alle Einstellungen in untergeordneten `li`-Elementen.</span><span class="sxs-lookup"><span data-stu-id="90932-154">The `data-tag` setting for a `ul` or `ol` overrides all settings on child `li` elements.</span></span> <span data-ttu-id="90932-155">Dies gilt auch dann, wenn das `ul`- oder `ol`-Element kein `data-tag` angibt, aber seine untergeordneten `li`-Elemente dies tun.</span><span class="sxs-lookup"><span data-stu-id="90932-155">The data-tag`ul` setting for a ul`ol` or ol`data-tag` overrides all settings on child li`li` elements. This applies even when the ul or ol doesn't specify a data-tag but its child li elements do.</span></span>

   <span data-ttu-id="90932-156">Wenn Sie beispielsweise ein `ul`- oder `ol`-Element erstellen, das `data-tag="project-a"` definiert, zeigen alle Listenelemente das Notiztag *Project A* an.</span><span class="sxs-lookup"><span data-stu-id="90932-156">For example, if you create a `ul` or `ol` that defines `data-tag="project-a"`, all its list items will display the *Project A* note tag.</span></span> <span data-ttu-id="90932-157">Wenn dagegen das `ul`- oder `ol`-Element kein `data-tag` definiert, zeigt keines seiner Elemente ein Notiztag an.</span><span class="sxs-lookup"><span data-stu-id="90932-157">Or if the `ul` or `ol` doesn't define a `data-tag`, none of its items will display a note tag.</span></span> <span data-ttu-id="90932-158">Diese Außerkraftsetzung geschieht unabhängig von expliziten Einstellungen in untergeordneten `li`-Elementen.</span><span class="sxs-lookup"><span data-stu-id="90932-158">This override happens regardless of any explicit settings on child `li` elements.</span></span>

- <span data-ttu-id="90932-159">Eindeutige `data-tag`-Einstellungen werden für Listenelemente unter den folgenden Bedingungen berücksichtigt:</span><span class="sxs-lookup"><span data-stu-id="90932-159">Unique data-tag`data-tag` settings are honored for list items under the following conditions:</span></span>

   - <span data-ttu-id="90932-160">Die `li`-Elemente sind nicht in einem `ul` oder `ol` in einer Erstellungs- oder Aktualisierungsanforderung geschachtelt.</span><span class="sxs-lookup"><span data-stu-id="90932-160">The li`li` elements are not nested in a ul`ul` or ol`ol` in a create or update request (see example below).</span></span>

   - <span data-ttu-id="90932-161">Ein `li`-Element wird einzeln in einer Aktualisierungsanforderung adressiert.</span><span class="sxs-lookup"><span data-stu-id="90932-161">An li`li` element is individually addressed in an update request.</span></span>

- <span data-ttu-id="90932-162">Ungeschachtelte `li`-Elemente, die im Eingabe-HTML-Code gesendet wurden, werden in einem `ul` im Ausgabe-HTML-Code zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="90932-162">Unnested li`li` elements sent in input HTML are returned in a ul`ul` in the output HTML (see example below).</span></span>

- <span data-ttu-id="90932-163">Im Ausgabe-HTML-Code werden alle `data-tag`-Listeneinstellungen in `span`-Elementen für die Listenelemente definiert.</span><span class="sxs-lookup"><span data-stu-id="90932-163">In output HTML, all `data-tag` list settings are defined on `span` elements on the list items.</span></span>

<br />
<span data-ttu-id="90932-164">Der folgende Code zeigt, wie einige dieser Regeln angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="90932-164">The following code shows how some of these rules are applied.</span></span> <span data-ttu-id="90932-165">Der Eingabe-HTML-Code erstellt zwei Listen mit Notiztags.</span><span class="sxs-lookup"><span data-stu-id="90932-165">The input HTML creates two lists with note tags.</span></span> <span data-ttu-id="90932-166">Der Ausgabe-HTML-Code wird für die Listen zurückgegeben, wenn Sie den Inhalt der Seite abrufen.</span><span class="sxs-lookup"><span data-stu-id="90932-166">The output HTML is what's returned for the lists when you retrieve page content.</span></span>

<span data-ttu-id="90932-167">**Eingabe-HTML-Code**</span><span class="sxs-lookup"><span data-stu-id="90932-167">**Input HTML**</span></span>

```html 
<!--To display the same note tag on all list items, define note tags on the ul or ol.--> 
<ul data-tag="project-a" data-id="agenda">
  <li>An item with a Project A note tag</li>
  <li>An item with a Project A note tag</li>
</ul>

<!--To display unique note tags on list items, don't nest li elements in a ul or ol.--> 
<li data-tag="idea" data-id="my-idea">An item with an Idea note tag</li>
<li data-tag="question" data-id="my-question">An item with a Question note tag</li>
```
 
<span data-ttu-id="90932-168">**Ausgabe-HTML-Code**</span><span class="sxs-lookup"><span data-stu-id="90932-168">**Output HTML**</span></span>

```html 
<ul>
  <li><span data-tag="project-a">An item with a Project A note tag</span></li>
  <li><span data-tag="project-a">An item with a Project A note tag</span></li>
</ul>
<br />
<ul>
  <li style="..."><span data-tag="idea">An item with an Idea note tag</span></li>
  <li style="..."><span data-tag="question">An item with a Question note tag</span></li>
</ul>
```

<a name="output-html"></a>
## <a name="retrieve-note-tags"></a><span data-ttu-id="90932-169">Abrufen von Notiztags</span><span class="sxs-lookup"><span data-stu-id="90932-169">Retrieve note tags</span></span>

<span data-ttu-id="90932-170">Integrierte Notiztags sind im Ausgabe-HTML-Code enthalten, wenn Sie Seiteninhalte abrufen:</span><span class="sxs-lookup"><span data-stu-id="90932-170">Built-in note tags are included in the output HTML when you retrieve page content by sending a GET request to the content endpoint:</span></span>

`GET ../api/v1.0/pages/{page-id}/content` 

<span data-ttu-id="90932-171">Ein `data-tag`-Attribut in der HTML-Ausgabe enthält immer einen Shape-Wert. Zusätzlich ist ein Status enthalten, wenn es sich um ein Kontrollkästchen-Notiztag handelt, das auf „completed“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="90932-171">The data-tag attribute in the output HTML always includes the shape value, and it only includes  status if it represents a check-box note tag that's  set to completed. The following examples show the input HTML used to create some note tags and the output HTML that's returned.</span></span> <span data-ttu-id="90932-172">Das folgende Beispiel zeigt den Eingabe-HTML-Code, der zum Erstellen einiger Notiztags verwendet wurde, und den zurückgegebenen Ausgabe-HTML-Code.</span><span class="sxs-lookup"><span data-stu-id="90932-172">The following examples show the input HTML used to create some note tags and the output HTML that's returned.</span></span>

<span data-ttu-id="90932-173">**Eingabe-HTML-Code**</span><span class="sxs-lookup"><span data-stu-id="90932-173">**Input HTML**</span></span>

```html 
<h1>Status meeting</h1>
<p data-tag="important">Next week's meeting has been moved to <b>Wednesday</b>.</p>
<p data-tag="question">What are the exact dates for the conference?</p>
<p>Upcoming training opportunities. See Katie for more info.</p>
<p data-tag="project-a">Around the room updates.</p>
<ul data-tag="critical">
  <li>Design handouts</li>
  <li>Plan keynote</li>
</ul>
```

<span data-ttu-id="90932-174">**Ausgabe-HTML-Code**</span><span class="sxs-lookup"><span data-stu-id="90932-174">**Output HTML**</span></span>

```html 
<h1 style="...">Status meeting</h1>
<p data-tag="important">Next week's meeting has been moved to <span style="font-weight:bold">Wednesday</span>.</p>
<p data-tag="question">What are the exact dates for the conference?</p>
<p>Upcoming training opportunities. See Katie for more info.</p>
<p data-tag="project-a">Around the room updates.</p>
<ul>
  <li><span data-tag="critical">Design handouts</span></li>
  <li><span data-tag="critical">Plan keynote</span></li>
</ul>
```

<span data-ttu-id="90932-175">Beachten Sie, dass das auf Listenebene definierte `data-tag`-Attribut auf dessen Listenelemente übertragen wird.</span><span class="sxs-lookup"><span data-stu-id="90932-175">Note that the data-tag`data-tag` attribute defined at the list level is pushed to its list items. For more information about using note tags with lists, see Note tags on lists.</span></span> <span data-ttu-id="90932-176">Weitere Informationen zur Verwendung von Notiztags mit Listen finden Sie unter [Notiztags in Listen](#note-tags-on-lists).</span><span class="sxs-lookup"><span data-stu-id="90932-176">Note that the data-tag attribute defined at the list level is pushed to its list items. For more information about using note tags with lists, see [Note tags on lists](#note-tags-on-lists).</span></span>

> <span data-ttu-id="90932-177">**Hinweis:** Im HTML-Ausgabe-Code werden die Notiztags für Definition und Speicherung als `data-tag="remember-for-later"` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="90932-177">**Note:** In the output HTML, the definition and remember-for-later note tags are both returned as `data-tag="remember-for-later"`.</span></span> <span data-ttu-id="90932-178">Das `title`-Element gibt keine Notiztaginformationen zurück.</span><span class="sxs-lookup"><span data-stu-id="90932-178">element doesn't return any note tag information.</span></span>

<a name="built-in-tags"></a>
## <a name="built-in-note-tags-for-onenote"></a><span data-ttu-id="90932-179">Integrierte Notiztags für OneNote</span><span class="sxs-lookup"><span data-stu-id="90932-179">Built-in note tags for onnvshort</span></span>

<span data-ttu-id="90932-180">OneNote umfasst die folgenden integrierten Notiztags:</span><span class="sxs-lookup"><span data-stu-id="90932-180">onnvshort  includes the following built-in  note tags:</span></span>

![Alle integrierten Notiztags.](images/note-tags-all.png)

<span data-ttu-id="90932-182">Die Werte, die Sie dem `data-tag`-Attribut zuweisen können, werden im Folgenden aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="90932-182">The values you can assign to the data-tag`data-tag` attribute are shown below.</span></span> <span data-ttu-id="90932-183">Benutzerdefinierte Tags werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="90932-183">Custom tags are not supported.</span></span>

||<span data-ttu-id="90932-184">Tags</span><span class="sxs-lookup"><span data-stu-id="90932-184">Tags</span></span>||
|:---|:---|:-----|
| `shape[:status]` |`to-do`<br />`to-do:completed`|`important`|
|`question`|`definition`|`highlight`|
|`contact`|`address`|`phone-number`|
|`web-site-to-visit`|`idea`|`password`|
|`critical`|`project-a`|`project-b`|
|`remember-for-later`|`movie-to-see`|`book-to-read`|
|`music-to-listen-to`|`source-for-article`|`remember-for-blog`|
|`discuss-with-person-a`<br />`discuss-with-person-a:completed`|`discuss-with-person-b`<br />`discuss-with-person-b:completed`|`discuss-with-manager`<br />`discuss-with-manager:completed`|
|`send-in-email`|`schedule-meeting`<br />`schedule-meeting:completed`|`call-back`<br />`call-back:completed`|
|`to-do-priority-1`<br />`to-do-priority-1:completed`|`to-do-priority-2`<br />`to-do-priority-2:completed`|`client-request`<br />`client-request:completed`|


<a name="request-response-info"></a>
## <a name="response-information"></a><span data-ttu-id="90932-185">Antwortinformationen</span><span class="sxs-lookup"><span data-stu-id="90932-185">Response information</span></span>
<span data-ttu-id="90932-186">Microsoft Graph gibt die folgenden Informationen in der Antwort zurück.</span><span class="sxs-lookup"><span data-stu-id="90932-186">The onnvshort API returns the following information in the response.</span></span>

| <span data-ttu-id="90932-187">Antwortdaten</span><span class="sxs-lookup"><span data-stu-id="90932-187">Response data</span></span> | <span data-ttu-id="90932-188">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90932-188">Description</span></span> |  
|------|------|  
| <span data-ttu-id="90932-189">Erfolgscode</span><span class="sxs-lookup"><span data-stu-id="90932-189">Success code</span></span> | <span data-ttu-id="90932-190">HTTP-Statuscode 201 für eine erfolgreiche POST-Anforderung, HTTP-Statuscode 204 für eine erfolgreiche PATCH-Anforderung.</span><span class="sxs-lookup"><span data-stu-id="90932-190">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="90932-191">Fehler</span><span class="sxs-lookup"><span data-stu-id="90932-191">Errors</span></span> | <span data-ttu-id="90932-192">Weitere Informationen zu OneNote-Fehlern, die Microsoft Graph zurückgeben kann, finden Sie unter [Fehlercodes für OneNote-APIs in Microsoft Graph](onenote_error_codes.md).</span><span class="sxs-lookup"><span data-stu-id="90932-192">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  


<a name="permissions"></a>
## <a name="permissions"></a><span data-ttu-id="90932-193">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="90932-193">Permissions</span></span>

<span data-ttu-id="90932-194">Zum Erstellen oder Aktualisieren von OneNote-Seiten müssen Sie die entsprechenden Berechtigungen anfordern.</span><span class="sxs-lookup"><span data-stu-id="90932-194">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="90932-195">Wählen Sie die niedrigste Berechtigungsstufe, die Ihre App zur Erledigung ihrer Aufgaben benötigt.</span><span class="sxs-lookup"><span data-stu-id="90932-195">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="90932-196">**Berechtigungen für _POST Pages_**</span><span class="sxs-lookup"><span data-stu-id="90932-196">**Permissions for _POST pages_**</span></span>

- <span data-ttu-id="90932-197">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="90932-197">Notes.Create</span></span>
- <span data-ttu-id="90932-198">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90932-198">Notes.ReadWrite</span></span>
- <span data-ttu-id="90932-199">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90932-199">Notes.ReadWrite.All</span></span>  

<span data-ttu-id="90932-200">**Berechtigungen für _PATCH Pages_**</span><span class="sxs-lookup"><span data-stu-id="90932-200">**Permissions for _PATCH pages_**</span></span>

- <span data-ttu-id="90932-201">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90932-201">Notes.ReadWrite</span></span>
- <span data-ttu-id="90932-202">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90932-202">Notes.ReadWrite.All</span></span>  

<span data-ttu-id="90932-203">Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie unter [OneNote-Berechtigungsbereiche](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="90932-203">For more information about how permission scopes work, see [OneNote permission scopes](permissions_reference.md).</span></span>


<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="90932-204">Weitere Ressourcen</span><span class="sxs-lookup"><span data-stu-id="90932-204">Additional resources</span></span>

- [<span data-ttu-id="90932-205">Erstellen von OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="90932-205">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="90932-206">Aktualisieren von OneNote-Seiteninhalten</span><span class="sxs-lookup"><span data-stu-id="90932-206">Update OneNote page content</span></span>](onenote_update_page.md)
- [<span data-ttu-id="90932-207">Integrieren in OneNote</span><span class="sxs-lookup"><span data-stu-id="90932-207">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="90932-208">OneNote-Entwicklerblog</span><span class="sxs-lookup"><span data-stu-id="90932-208">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="90932-209">Fragen zur OneNote-Entwicklung auf Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="90932-209">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="90932-210">OneNote GitHub-Repos</span><span class="sxs-lookup"><span data-stu-id="90932-210">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
 


