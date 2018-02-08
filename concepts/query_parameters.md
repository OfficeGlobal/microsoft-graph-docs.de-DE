# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="e6bef-101">Verwenden von Abfrageparametern zum Anpassen von Antworten</span><span class="sxs-lookup"><span data-stu-id="e6bef-101">Use query parameters to customize responses</span></span>

<span data-ttu-id="e6bef-p101">Microsoft Graph stellt optionale Abfrageparameter bereit, die Sie zum Festlegen und Steuern der in einer Antwort zurückgegebenen Datenmenge verwenden können. Die folgenden Abfrageparameter werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e6bef-p101">Microsoft Graph provides optional query parameters that you can use to specify and control the amount of data returned in a response. The following query parameters are supported.</span></span>

><span data-ttu-id="e6bef-104">**Hinweis:** Klicken Sie auf die Beispiele, um sie im [Graph-Tester][graph-explorer] auszuprobieren.</span><span class="sxs-lookup"><span data-stu-id="e6bef-104">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="e6bef-105">Name</span><span class="sxs-lookup"><span data-stu-id="e6bef-105">Name</span></span>                     | <span data-ttu-id="e6bef-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6bef-106">Description</span></span> | <span data-ttu-id="e6bef-107">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6bef-107">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="e6bef-108">$count</span><span class="sxs-lookup"><span data-stu-id="e6bef-108">$count</span></span>](#count-parameter)         | <span data-ttu-id="e6bef-109">Dient zum Abrufen der Gesamtzahl übereinstimmender Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="e6bef-109">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="e6bef-110">$expand</span><span class="sxs-lookup"><span data-stu-id="e6bef-110">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="e6bef-111">Dient zum Abrufen von verwandten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="e6bef-111">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="e6bef-112">$filter</span><span class="sxs-lookup"><span data-stu-id="e6bef-112">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="e6bef-113">Dient zum Filtern von Ergebnissen (Zeilen).</span><span class="sxs-lookup"><span data-stu-id="e6bef-113">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="e6bef-114">$format</span><span class="sxs-lookup"><span data-stu-id="e6bef-114">$format</span></span>](#format-parameter)       | <span data-ttu-id="e6bef-115">Dient zum Zurückgeben der Ergebnisse im angegebenen Medienformat.</span><span class="sxs-lookup"><span data-stu-id="e6bef-115">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="e6bef-116">$orderby</span><span class="sxs-lookup"><span data-stu-id="e6bef-116">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="e6bef-117">Dient zum Sortieren von Ergebnissen.</span><span class="sxs-lookup"><span data-stu-id="e6bef-117">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="e6bef-118">$search</span><span class="sxs-lookup"><span data-stu-id="e6bef-118">$search</span></span>](#search-parameter)       | <span data-ttu-id="e6bef-p102">Dient zum Zurückgeben von Ergebnissen basierend auf Suchkriterien. Wird derzeit in **messages**- und **person**-Sammlungen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e6bef-p102">Returns results based on search criteria. Currently supported on **messages** and **person** collections.</span></span>|[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="e6bef-121">$select</span><span class="sxs-lookup"><span data-stu-id="e6bef-121">$select</span></span>](#select-parameter)       | <span data-ttu-id="e6bef-122">Dient zum Filtern von Eigenschaften (Spalten).</span><span class="sxs-lookup"><span data-stu-id="e6bef-122">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="e6bef-123">$skip</span><span class="sxs-lookup"><span data-stu-id="e6bef-123">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="e6bef-p103">Dient zum Indizieren in einem Resultset. Wird auch von einigen APIs zum Implementieren von Paging verwendet und kann zusammen mit `$top` zum manuellen Auslagern von Ergebnissen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="e6bef-p103">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="e6bef-126">$skipToken</span><span class="sxs-lookup"><span data-stu-id="e6bef-126">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="e6bef-p104">Dient zum Abrufen der nächsten Seite von Ergebnissen aus Resultsets, die mehrere Seiten umfassen. (Einige APIs verwenden stattdessen `$skip`.)</span><span class="sxs-lookup"><span data-stu-id="e6bef-p104">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|
| [<span data-ttu-id="e6bef-129">$top</span><span class="sxs-lookup"><span data-stu-id="e6bef-129">$top</span></span>](#top-parameter)             | <span data-ttu-id="e6bef-130">Dient zum Festlegen der Seitengröße von Ergebnissen.</span><span class="sxs-lookup"><span data-stu-id="e6bef-130">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]



<span data-ttu-id="e6bef-131">Diese Parameter sind mit der [OData V4-Abfragesprache][odata-query] kompatibel.</span><span class="sxs-lookup"><span data-stu-id="e6bef-131">These parameters are compatible with the [OData V4 query language][odata-query].</span></span> <span data-ttu-id="e6bef-132">Nicht alle Parameter werden über alle Microsoft Graph-APIs hinweg unterstützt, und die Unterstützung kann zwischen dem `v1.0`- und dem `beta`-Endpunkt erheblich abweichen.</span><span class="sxs-lookup"><span data-stu-id="e6bef-132">Not all parameters are supported across all Microsoft Graph APIs, and support might differ significantly between the `v1.0` and `beta` endpoints.</span></span> 

> <span data-ttu-id="e6bef-p106">**Hinweis:** Am `beta`-Endpunkt ist das `$`-Präfix optional. Sie können z. B. `filter` anstelle von `$filter` verwenden. Weitere Informationen und Beispiele finden Sie unter [Abfrageparameter ohne $ Präfixe in Microsoft Graph unterstützen](http://dev.office.com/queryparametersinMicrosoftGraph).</span><span class="sxs-lookup"><span data-stu-id="e6bef-p106">**Note:** On the `beta` endpoint, the `$` prefix is optional. For example, instead of `$filter`, you can use `filter`. For more details and examples, see [Supporting query parameters without $ prefixes in Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).</span></span>

## <a name="encoding-query-parameters"></a><span data-ttu-id="e6bef-136">Codieren von Abfrageparametern</span><span class="sxs-lookup"><span data-stu-id="e6bef-136">Encoding query parameters</span></span>

<span data-ttu-id="e6bef-137">Die Werte von Abfrageparametern sollten als Prozentwert codiert werden.</span><span class="sxs-lookup"><span data-stu-id="e6bef-137">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="e6bef-138">Viele HTTP-Clients, Browser und Tools (z. B. der [Graph-Tester][graph-explorer]) sind Ihnen dabei behilflich.</span><span class="sxs-lookup"><span data-stu-id="e6bef-138">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="e6bef-139">Wenn bei einer Abfrage ein Fehler auftritt, kann eine der möglichen Ursachen dafür sein, dass die Werte von Abfrageparametern nicht ordnungsgemäß codiert wurden.</span><span class="sxs-lookup"><span data-stu-id="e6bef-139">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="e6bef-140">Eine nicht codierte URL sieht folgendermaßen aus:</span><span class="sxs-lookup"><span data-stu-id="e6bef-140">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="e6bef-141">Eine korrekt codierte URL sieht folgendermaßen aus:</span><span class="sxs-lookup"><span data-stu-id="e6bef-141">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count-parameter"></a><span data-ttu-id="e6bef-142">count-Parameter</span><span class="sxs-lookup"><span data-stu-id="e6bef-142">count parameter</span></span>

<span data-ttu-id="e6bef-143">Verwenden Sie `$count` als Abfrageparameter, um die Gesamtzahl der Elemente in einer Sammlung zusammen mit der Seite der Datenwerte anzugeben, die von Microsoft Graph zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="e6bef-143">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="e6bef-144">Die folgende Anforderung gibt beispielsweise sowohl die **contact**-Sammlung des aktuellen Benutzers sowie die Anzahl von Elementen in der **contact**-Sammlung in der `@odata.count`-Eigenschaft zurück.</span><span class="sxs-lookup"><span data-stu-id="e6bef-144">For example, the following request will return both the **contact** collection of the current user, and the number of items in the **contact** collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="e6bef-145">Im Graph-Tester ausprobieren</span><span class="sxs-lookup"><span data-stu-id="e6bef-145">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


><span data-ttu-id="e6bef-146">**Hinweis:** `$count` wird für Sammlungen von Ressourcen, die von [directoryObject](../api-reference/v1.0/resources/directoryobject.md) abgeleitet werden, wie Sammlungen von [Benutzern](../api-reference/v1.0/resources/user.md) oder [Gruppen](../api-reference/v1.0/resources/group.md), nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e6bef-146">**Note:** `$count` is not supported for collections of resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md) like collections of [users](../api-reference/v1.0/resources/user.md) or [groups](../api-reference/v1.0/resources/group.md).</span></span>

## <a name="expand-parameter"></a><span data-ttu-id="e6bef-147">expand-Parameter</span><span class="sxs-lookup"><span data-stu-id="e6bef-147">expand parameter</span></span>

<span data-ttu-id="e6bef-148">Viele Microsoft Graph-Ressourcen machen sowohl deklarierte Eigenschaften der Ressource als auch deren Beziehungen zu anderen Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="e6bef-148">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="e6bef-149">Diese Beziehungen werden auch als Verweiseigenschaften oder Navigationseigenschaften bezeichnet und können auf eine einzelne Ressource oder auf eine Sammlung von Ressourcen verweisen.</span><span class="sxs-lookup"><span data-stu-id="e6bef-149">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="e6bef-150">Beispielsweise werden die E-Mail-Ordner, die Vorgesetzten und die direkten Mitarbeiter eines Benutzers alle als Beziehungen verfügbar gemacht.</span><span class="sxs-lookup"><span data-stu-id="e6bef-150">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="e6bef-p109">Normalerweise können Sie die Eigenschaften einer Ressource oder eine ihrer Beziehungen in einer einzelnen Anforderung abfragen, aber nicht beides gleichzeitig. Sie können den `$expand`-Zeichenfolgen-Abfrageparameter verwenden, um die erweiterte Ressource oder die Sammlung, auf die von einer einzigen Beziehung verwiesen wird (Navigationseigenschaft) in Ihre Ergebnisse einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="e6bef-p109">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="e6bef-153">Im folgenden Beispiel werden Informationen des Stammlaufwerks zusammen mit den untergeordneten Elementen der obersten Ebene in einem Laufwerk abgerufen:</span><span class="sxs-lookup"><span data-stu-id="e6bef-153">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="e6bef-154">Im Graph-Tester ausprobieren</span><span class="sxs-lookup"><span data-stu-id="e6bef-154">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="e6bef-p110">Bei einigen Ressourcensammlungen können Sie auch die Eigenschaften angeben, die in den erweiterten Ressourcen zurückgegeben werden sollen, indem Sie einen `$select`-Parameter hinzufügen. Im folgenden Beispiel wird die gleiche Abfrage wie im vorherigen Beispiel ausgeführt, hier wird jedoch eine [`$select`](#select-parameter)-Anweisung verwendet, um die für die erweiterten untergeordneten Elemente zurückgegebenen Eigenschaften auf die **id**- und **name**-Eigenschaften einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="e6bef-p110">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **id** and **name** properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="e6bef-157">[Ausprobieren im Graph-Tester][expand-example]</span><span class="sxs-lookup"><span data-stu-id="e6bef-157">[Try in Graph Explorer][expand-example]</span></span>

> <span data-ttu-id="e6bef-p111">**Hinweis:** Nicht alle Beziehungen und Ressourcen unterstützen den `$expand`-Abfrageparameter. Sie können z. B. die Beziehungen **directReports**, **manager** und **memberOf** für einen Benutzer erweitern, aber Sie können nicht seine Beziehungen **events**, **messages** oder **photo** erweitern. Nicht alle Ressourcen oder Beziehungen unterstützen die Verwendung von `$select` in erweiterten Elementen.</span><span class="sxs-lookup"><span data-stu-id="e6bef-p111">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the **directReports**, **manager**, and **memberOf** relationships on a user, but you cannot expand its **events**, **messages**, or **photo** relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="e6bef-161">Bei Azure AD-Ressourcen, die von [directoryObject](../api-reference/v1.0/resources/directoryobject.md) abgeleitet werden, z. B. [Benutzer](../api-reference/v1.0/resources/user.md) und [Gruppe](../api-reference/v1.0/resources/group.md), wird `$expand` nur für `beta` unterstützt, und es werden maximal 20 Elemente für die erweiterte Beziehung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6bef-161">With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="e6bef-162">filter-Parameter</span><span class="sxs-lookup"><span data-stu-id="e6bef-162">filter parameter</span></span>

<span data-ttu-id="e6bef-163">Verwenden Sie den `$filter`-Abfrageparameter, um nur eine Teilmenge einer Sammlung abzurufen.</span><span class="sxs-lookup"><span data-stu-id="e6bef-163">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> 

<span data-ttu-id="e6bef-164">Um beispielsweise Benutzer zu suchen, deren Anzeigename mit dem Buchstaben „J“ beginnt, verwenden Sie `startswith`.</span><span class="sxs-lookup"><span data-stu-id="e6bef-164">For example, to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="e6bef-165">[Ausprobieren im Graph-Tester][filter-example]</span><span class="sxs-lookup"><span data-stu-id="e6bef-165">[Try in Graph Explorer][filter-example]</span></span>

<span data-ttu-id="e6bef-166">Die Unterstützung für `$filter`-Operatoren variiert je nach Microsoft Graph-API.</span><span class="sxs-lookup"><span data-stu-id="e6bef-166">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="e6bef-167">Im Allgemeinen werden die folgenden logischen Operatoren unterstützt:</span><span class="sxs-lookup"><span data-stu-id="e6bef-167">The following logical operators are generally supported:</span></span> 

- <span data-ttu-id="e6bef-168">gleich (`eq`)</span><span class="sxs-lookup"><span data-stu-id="e6bef-168">equals (`eq`)</span></span>
- <span data-ttu-id="e6bef-169">ungleich (`ne`)</span><span class="sxs-lookup"><span data-stu-id="e6bef-169">not equals (`ne`)</span></span>
- <span data-ttu-id="e6bef-170">größer als (`gt`)</span><span class="sxs-lookup"><span data-stu-id="e6bef-170">greater than (`gt`)</span></span>
- <span data-ttu-id="e6bef-171">größer als oder gleich (`ge`)</span><span class="sxs-lookup"><span data-stu-id="e6bef-171">greater than or equals (`ge`)</span></span>
- <span data-ttu-id="e6bef-172">kleiner als (`lt`), kleiner als oder gleich (`le`)</span><span class="sxs-lookup"><span data-stu-id="e6bef-172">less than (`lt`), less than or equals (`le`)</span></span>
- <span data-ttu-id="e6bef-173">und (`and`)</span><span class="sxs-lookup"><span data-stu-id="e6bef-173">and (`and`)</span></span>
- <span data-ttu-id="e6bef-174">oder (`or`)</span><span class="sxs-lookup"><span data-stu-id="e6bef-174">or (`or`)</span></span>
- <span data-ttu-id="e6bef-175">nicht (`not`)</span><span class="sxs-lookup"><span data-stu-id="e6bef-175">not (`not`)</span></span>
 
<span data-ttu-id="e6bef-176">Der Zeichenfolgenoperator `startswith` wird häufig unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e6bef-176">The `startswith` string operator is often supported.</span></span> <span data-ttu-id="e6bef-177">Der Lambda-Operator `any` wird für einige APIs unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e6bef-177">The `any` lambda operator is supported for some APIs.</span></span> <span data-ttu-id="e6bef-178">In der folgenden Tabelle finden Sie einige Verwendungsbeispiele.</span><span class="sxs-lookup"><span data-stu-id="e6bef-178">For some  usage examples, see the following table.</span></span> <span data-ttu-id="e6bef-179">Weitere Informationen zur `$filter`-Syntax finden Sie im [OData-Protokoll][odata-filter].</span><span class="sxs-lookup"><span data-stu-id="e6bef-179">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="e6bef-180">Die folgende Tabelle enthält einige Beispiele zur Verwendung des `$filter`-Abfrageparameters.</span><span class="sxs-lookup"><span data-stu-id="e6bef-180">The following table shows some examples that use the `$filter` query parameter.</span></span>

> <span data-ttu-id="e6bef-181">**Hinweis:** Klicken Sie auf die Beispiele, um sie im [Graph-Tester][graph-explorer] auszuprobieren.</span><span class="sxs-lookup"><span data-stu-id="e6bef-181">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="e6bef-182">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6bef-182">Description</span></span> | <span data-ttu-id="e6bef-183">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6bef-183">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="e6bef-184">In mehreren Eigenschaften nach Benutzern mit dem Namen „Mary“ suchen</span><span class="sxs-lookup"><span data-stu-id="e6bef-184">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) 
| <span data-ttu-id="e6bef-185">Alle Ereignisse des angemeldeten Benutzers abrufen, die nach dem 01.07.2017 beginnen</span><span class="sxs-lookup"><span data-stu-id="e6bef-185">Get all the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) 
| <span data-ttu-id="e6bef-186">Alle E-Mails von einer bestimmten Adresse abrufen, die der angemeldete Benutzer erhalten hat</span><span class="sxs-lookup"><span data-stu-id="e6bef-186">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) 
| <span data-ttu-id="e6bef-187">Alle E-Mails abrufen, die der angemeldete Benutzer im April 2017 erhalten hat</span><span class="sxs-lookup"><span data-stu-id="e6bef-187">Get all emails received by the signed-in user in April 2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) 
| <span data-ttu-id="e6bef-188">Alle ungelesenen E-Mails im Postfach des angemeldeten Benutzers abrufen</span><span class="sxs-lookup"><span data-stu-id="e6bef-188">Get all unread mail in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) 
| <span data-ttu-id="e6bef-189">Alle Office 365-Gruppen in einer Organisation auflisten</span><span class="sxs-lookup"><span data-stu-id="e6bef-189">List all Office 365 groups in an organization.</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) 

> <span data-ttu-id="e6bef-p114">**Hinweis:** Die folgenden `$filter`-Operatoren werden für Azure AD-Ressourcen nicht unterstützt: `ne`, `gt`, `ge`, `lt`, `le` und `not`. Der `contains`-Zeichenfolgenoperator wird derzeit nicht für Microsoft Graph-Ressourcen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e6bef-p114">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="format-parameter"></a><span data-ttu-id="e6bef-192">format-Parameter</span><span class="sxs-lookup"><span data-stu-id="e6bef-192">format parameter</span></span>

<span data-ttu-id="e6bef-193">Verwenden Sie zum Festlegen des Medienformats der von Microsoft Graph zurückgegebenen Elemente den `$format`-Abfrageparameter.</span><span class="sxs-lookup"><span data-stu-id="e6bef-193">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="e6bef-194">Die folgende Anforderung gibt beispielsweise die Benutzer in der Organisation im JSON-Format zurück:</span><span class="sxs-lookup"><span data-stu-id="e6bef-194">For example, the following request returns the users in the organization in the json format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

<span data-ttu-id="e6bef-195">[Ausprobieren im Graph-Tester][format-example]</span><span class="sxs-lookup"><span data-stu-id="e6bef-195">[Try in Graph Explorer][format-example]</span></span>

> <span data-ttu-id="e6bef-196">**Hinweis:** Der `$format`-Abfrageparameter unterstützt eine Reihe von Formaten (z. B. Atom, XML und JSON), die Ergebnisse werden aber möglicherweise nicht in allen Formaten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6bef-196">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="e6bef-197">orderby-Parameter</span><span class="sxs-lookup"><span data-stu-id="e6bef-197">orderby parameter</span></span>

<span data-ttu-id="e6bef-198">Verwenden Sie zum Festlegen der Sortierreihenfolge der von Microsoft Graph zurückgegebenen Elemente den `$orderby`-Abfrageparameter.</span><span class="sxs-lookup"><span data-stu-id="e6bef-198">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="e6bef-199">Die folgende Anforderung gibt beispielsweise die Benutzer in der Organisation sortiert nach ihrem Anzeigenamen zurück:</span><span class="sxs-lookup"><span data-stu-id="e6bef-199">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
<span data-ttu-id="e6bef-200">[Ausprobieren im Graph-Tester][orderby-example]</span><span class="sxs-lookup"><span data-stu-id="e6bef-200">[Try in Graph Explorer][orderby-example]</span></span>

<span data-ttu-id="e6bef-p115">Sie können auch nach komplexen Typentitäten sortieren. In der folgenden Anforderung werden Nachrichten abgerufen und nach dem **Adresse**-Feld der **from**-Eigenschaft sortiert, die vom komplexen Typ **emailAddress** ist:</span><span class="sxs-lookup"><span data-stu-id="e6bef-p115">You can also sort by complex type entities. The following request gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="e6bef-203">Im Graph-Tester ausprobieren</span><span class="sxs-lookup"><span data-stu-id="e6bef-203">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="e6bef-204">Wenn Sie die Ergebnisse in aufsteigender oder absteigender Reihenfolge sortieren möchten, fügen Sie entweder `asc` oder `desc` getrennt durch ein Leerzeichen an den Namen des Felds an, z. B. `?$orderby=name%20desc`.</span><span class="sxs-lookup"><span data-stu-id="e6bef-204">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="e6bef-205">Bei einigen APIs können Sie die Ergebnisse anhand mehrerer Eigenschaften sortieren.</span><span class="sxs-lookup"><span data-stu-id="e6bef-205">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="e6bef-206">Die folgende Anforderung sortiert die Nachrichten im Posteingang des Benutzers beispielsweise zuerst nach dem Namen der Person, die die Nachricht gesendet hat, in absteigender Reihenfolge (von Z nach A) und anschließend nach dem Betreff in aufsteigender Reihenfolge (Standard).</span><span class="sxs-lookup"><span data-stu-id="e6bef-206">For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[<span data-ttu-id="e6bef-207">Im Graph-Tester ausprobieren</span><span class="sxs-lookup"><span data-stu-id="e6bef-207">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

<span data-ttu-id="e6bef-208">Wenn Sie $filter angeben, leitet der Server eine Sortierreihenfolge für die Ergebnisse ab.</span><span class="sxs-lookup"><span data-stu-id="e6bef-208">When you specify $filter the server will infer a sort order for the results.</span></span> <span data-ttu-id="e6bef-209">Wenn Sie sowohl `$orderby` als auch `$filter` verwenden, müssen die Eigenschaften in der `$filter` zuerst in der `$orderby` vor allen anderen Eigenschaften aufgeführt werden, und sie müssen in der Reihenfolge aufgeführt werden, in der sie im Parameter `$filter` angezeigt werden, da der Server immer eine Sortierreihenfolge für die Ergebnisse eines `$filter` ableitet.</span><span class="sxs-lookup"><span data-stu-id="e6bef-209">If you use both `$orderby` and `$filter`, because the server always infers a sort order for the results of a `$filter`, the properties in the `$filter` must be listed first in the `$orderby` before any other properties, and they must be listed in the order that they appear in the `$filter` parameter.</span></span> 

<span data-ttu-id="e6bef-210">Das folgende Beispiel zeigt eine Abfrage, die nach den Eigenschaften **subject** und **importance** gefiltert ist und dann nach den Eigenschaften **subject**, **importance** und **receivedDateTime** in absteigender Reihenfolge sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="e6bef-210">The following example shows a query filtered by the **subject** and **importance** properties, and then sorted by the **subject**, **importance**, and **receivedDateTime** properties in descending order.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome to exchange unified messaging' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[<span data-ttu-id="e6bef-211">Ausprobieren im Graph-Tester</span><span class="sxs-lookup"><span data-stu-id="e6bef-211">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome to exchange unified messaging%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

 > <span data-ttu-id="e6bef-212">**Hinweis:** Bei Azure AD-Ressourcen, die von [directoryObject](../api-reference/v1.0/resources/directoryobject.md) abgeleitet werden, wie z. B. [Benutzer](../api-reference/v1.0/resources/user.md) und [Gruppe](../api-reference/v1.0/resources/group.md), kann `$orderby` nicht mit `$filter`-Ausdrücken verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="e6bef-212">**Note:** With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search-parameter"></a><span data-ttu-id="e6bef-213">search-Parameter</span><span class="sxs-lookup"><span data-stu-id="e6bef-213">search parameter</span></span>

<span data-ttu-id="e6bef-214">Um die Ergebnisse einer Anforderung so zu beschränken, dass sie einem Suchkriterium entsprechen, verwenden Sie den `$search`-Abfrageparameter.</span><span class="sxs-lookup"><span data-stu-id="e6bef-214">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

> <span data-ttu-id="e6bef-p118">**Hinweis:** Sie können derzeit **nur** [Nachrichten](../api-reference/v1.0/resources/message.md)- und [Personen](../api-reference/v1.0/resources/person.md)-Sammlungen suchen. Eine `$search`-Anforderung gibt bis zu 250 Ergebnisse zurück. Sie können [`$filter`](#filter-parameter) oder [`$orderby`](#orderby-parameter) nicht in einer Suchabfrage verwenden.</span><span class="sxs-lookup"><span data-stu-id="e6bef-p118">**Note:** You can currently search **only** [message](../api-reference/v1.0/resources/message.md) and [person](../api-reference/v1.0/resources/person.md) collections. A `$search` request returns up to 250 results. You cannot use [`$filter`](#filter-parameter) or [`$orderby`](#orderby-parameter) in a search request.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="e6bef-218">Verwenden von $search in Nachrichtensammlungen</span><span class="sxs-lookup"><span data-stu-id="e6bef-218">Using $search on message collections</span></span>

<span data-ttu-id="e6bef-219">Office 365-Anwendungen wie Outlook und SharePoint unterstützen die KQL-Syntax (Keyword Query Language) für Suchvorgänge.</span><span class="sxs-lookup"><span data-stu-id="e6bef-219">Office 365 applications, such as Outlook and SharePoint, support the Keyword Query Language (KQL) syntax to do searches.</span></span> <span data-ttu-id="e6bef-220">Dies bietet den Vorteil einer gemeinsamen Discovery-Domäne für die Datenspeicher.</span><span class="sxs-lookup"><span data-stu-id="e6bef-220">This provides the convenience of a common discovery domain for their data stores.</span></span> 

<span data-ttu-id="e6bef-221">Beim Durchsuchen von Nachrichtensammlungen sind die Ergebnisse nach Datum und Uhrzeit sortiert, zu dem bzw. der die Nachricht gesendet wurde.</span><span class="sxs-lookup"><span data-stu-id="e6bef-221">When you search message collections, the results are sorted by the date and time that the message was sent.</span></span> 

<span data-ttu-id="e6bef-222">Sie können die folgenden Eigenschaften in einer **Nachricht** in einem `$search`-Kriterium angeben:</span><span class="sxs-lookup"><span data-stu-id="e6bef-222">You can specify the following properties on a **message** in a `$search` criterion:</span></span>

- <span data-ttu-id="e6bef-223">**attachments**</span><span class="sxs-lookup"><span data-stu-id="e6bef-223">**attachments**</span></span>
- <span data-ttu-id="e6bef-224">**bccRecipients**</span><span class="sxs-lookup"><span data-stu-id="e6bef-224">**bccRecipients**</span></span>
- <span data-ttu-id="e6bef-225">**body**</span><span class="sxs-lookup"><span data-stu-id="e6bef-225">**body**</span></span>
- <span data-ttu-id="e6bef-226">**category**</span><span class="sxs-lookup"><span data-stu-id="e6bef-226">**category**</span></span>
- <span data-ttu-id="e6bef-227">**ccRecipients**</span><span class="sxs-lookup"><span data-stu-id="e6bef-227">**ccRecipients**</span></span>
- <span data-ttu-id="e6bef-228">**content**</span><span class="sxs-lookup"><span data-stu-id="e6bef-228">**content**</span></span>
- <span data-ttu-id="e6bef-229">**from**</span><span class="sxs-lookup"><span data-stu-id="e6bef-229">**from**</span></span>
- <span data-ttu-id="e6bef-230">**hasAttachments**</span><span class="sxs-lookup"><span data-stu-id="e6bef-230">**hasAttachments**</span></span>
- <span data-ttu-id="e6bef-231">**participants**</span><span class="sxs-lookup"><span data-stu-id="e6bef-231">**participants**</span></span>
- <span data-ttu-id="e6bef-232">**receivedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e6bef-232">**receivedDateTime**</span></span>
- <span data-ttu-id="e6bef-233">**sender**</span><span class="sxs-lookup"><span data-stu-id="e6bef-233">**sender**</span></span>
- <span data-ttu-id="e6bef-234">**subject**</span><span class="sxs-lookup"><span data-stu-id="e6bef-234">**subject**</span></span>
- <span data-ttu-id="e6bef-235">**toRecipients**</span><span class="sxs-lookup"><span data-stu-id="e6bef-235">**toRecipients**</span></span>

<span data-ttu-id="e6bef-236">Wenn Sie eine Suche nach Nachrichten durchführen und nur einen Wert angeben, wird die Suche anhand der Standardsucheigenschaften**from**, **subject** und **body** ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="e6bef-236">If you do a search on messages and specify only a value, the search is carried out on the default search properties of **from**, **subject**, and **body**.</span></span>

<span data-ttu-id="e6bef-237">Im folgenden Beispiel werden alle Nachrichten im Posteingang des angemeldeten Benutzers zurückgegeben, die das Wort „Pizza“ in einer der drei Standardsucheigenschaften enthalten:</span><span class="sxs-lookup"><span data-stu-id="e6bef-237">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="e6bef-238">[Ausprobieren im Graph-Tester][search-example]</span><span class="sxs-lookup"><span data-stu-id="e6bef-238">[Try in Graph Explorer][search-example]</span></span>

<span data-ttu-id="e6bef-239">Im nächsten Beispiel werden alle Nachrichten im Posteingang des Benutzers, die von einer bestimmten E-Mail-Adresse gesendet wurden:</span><span class="sxs-lookup"><span data-stu-id="e6bef-239">The next example searches all messages in the user's Inbox that were sent from a specific email address:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```
<span data-ttu-id="e6bef-240">Weitere Informationen zu KQL, darunter zur Syntax, den unterstützten Operatoren und Tipps für die Suche finden Sie in den folgenden Artikeln:</span><span class="sxs-lookup"><span data-stu-id="e6bef-240">For more information about KQL such as the syntax, supported operators, and tips on searching, see the following articles:</span></span>

- [<span data-ttu-id="e6bef-241">Syntaxreferenz für die Keyword Query Language (KQL)</span><span class="sxs-lookup"><span data-stu-id="e6bef-241">Keyword Query Language (KQL) syntax reference</span></span>](https://docs.microsoft.com/de-DE/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- <span data-ttu-id="e6bef-242">
  [Nachrichteneigenschaften und Suchoperatoren für In-Situ-eDiscovery in Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span><span class="sxs-lookup"><span data-stu-id="e6bef-242">[Message properties and search operators for In-Place eDiscovery in Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span></span>

### <a name="using-search-on-person-collections"></a><span data-ttu-id="e6bef-243">Verwenden von $search in Personensammlungen</span><span class="sxs-lookup"><span data-stu-id="e6bef-243">Using $search on person collections</span></span>

<span data-ttu-id="e6bef-p120">Sie können die Personen-API von Microsoft Graph verwenden, um Personen abzurufen, die für einen Benutzer am relevantesten sind. Relevanz wird durch die Kommunikations- und Zusammenarbeitsmuster und Geschäftsbeziehungen des Benutzers bestimmt. Die Personen-API unterstützt den `$search`-Abfrageparameter.</span><span class="sxs-lookup"><span data-stu-id="e6bef-p120">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. The People API supports the `$search` query parameter.</span></span>

<span data-ttu-id="e6bef-247">Personensuchen werden sowohl für die Eigenschaft **displayName** als auch für die Eigenschaft **emailAddress** der Ressource vom Typ [person](../api-reference/v1.0/resources/person.md) ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="e6bef-247">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](../api-reference/v1.0/resources/person.md) resource.</span></span>

<span data-ttu-id="e6bef-248">Die folgende Anforderung führt eine Suche nach einer Person mit dem Namen „Irene McGowen“ in den Eigenschaften **displayName** und **emailAddress** für jede Person in der Sammlung **people** des angemeldeten Benutzers durch.</span><span class="sxs-lookup"><span data-stu-id="e6bef-248">The following request does a search for a person named "Irene McGowen" in the **displayName** and **emailAddress** properties in each person in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="e6bef-249">Da eine Person mit dem Namen „Irene McGowan“ für den angemeldeten Benutzer relevant ist, werden die Informationen für „Irene McGowan“ zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6bef-249">The following request does a search for a person named "Irene McGowen". Because a person named "Irene McGowan" is relevant to the signed-in user, the information for "Irene McGowan" is returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

<span data-ttu-id="e6bef-250">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="e6bef-250">The following example shows the response.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```

<span data-ttu-id="e6bef-251">Weitere Informationen zur Personen-API finden Sie unter [Abrufen von Informationen über die entsprechenden Personen](./people_example.md#search-people).</span><span class="sxs-lookup"><span data-stu-id="e6bef-251">To learn more about the People API, see [Get information about relevant people](./people_example.md#search-people).</span></span>  

## <a name="select-parameter"></a><span data-ttu-id="e6bef-252">select-Parameter</span><span class="sxs-lookup"><span data-stu-id="e6bef-252">select parameter</span></span>

<span data-ttu-id="e6bef-253">Verwenden Sie den `$select`-Abfrageparameter, um eine Reihe von Eigenschaften zurückzugeben, die sich von den Standardeigenschaften für eine einzelne Ressource oder eine Sammlung von Ressourcen unterscheidet.</span><span class="sxs-lookup"><span data-stu-id="e6bef-253">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="e6bef-254">Mit $select können Sie eine Teilmenge oder eine Obermenge der Standardeigenschaften angeben.</span><span class="sxs-lookup"><span data-stu-id="e6bef-254">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="e6bef-255">Wenn Sie z. B. die Nachrichten des angemeldeten Benutzers abrufen, können Sie angeben, dass nur die Eigenschaften **from** und **subject** zurückgegeben werden:</span><span class="sxs-lookup"><span data-stu-id="e6bef-255">For example, when retrieving the messages of the signed-in user, you can specify that only the **from** and **subject** properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<span data-ttu-id="e6bef-256">[Ausprobieren im Graph-Tester][select-example]</span><span class="sxs-lookup"><span data-stu-id="e6bef-256">[Try in Graph Explorer][select-example]</span></span>

> <span data-ttu-id="e6bef-257">**Wichtig:** Im Allgemeinen wird empfohlen, dass Sie `$select` verwenden, um die von einer Abfrage zurückgegebenen Eigenschaften auf diejenigen zu beschränken, die von Ihrer App benötigt werden.</span><span class="sxs-lookup"><span data-stu-id="e6bef-257">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="e6bef-258">Dies gilt insbesondere für Abfragen, die möglicherweise ein großes Resultset zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="e6bef-258">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="e6bef-259">Durch Beschränken der in den einzelnen Zeilen zurückgegebenen Eigenschaften werden die Netzwerklast reduziert und die Leistung Ihrer App verbessert.</span><span class="sxs-lookup"><span data-stu-id="e6bef-259">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="e6bef-p124">In `v1.0` geben einige Azure AD-Ressourcen, die von [directoryObject](../api-reference/v1.0/resources/directoryobject.md) abgeleitet werden, z.B. [Benutzer](../api-reference/v1.0/resources/user.md) und [Gruppe](../api-reference/v1.0/resources/group.md) eine begrenzte, standardmäßige Untermenge von Eigenschaften für Lesevorgänge zurück. Für diese Ressourcen müssen Sie `$select` verwenden, um Eigenschaften außerhalb des Standardsatzes zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="e6bef-p124">In `v1.0`, some Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="e6bef-262">skip-Parameter</span><span class="sxs-lookup"><span data-stu-id="e6bef-262">skip parameter</span></span>

<span data-ttu-id="e6bef-p125">Verwenden Sie den `$skip`-Abfrageparameter zum Festlegen der Anzahl der Elemente, die am Anfang einer Sammlung übersprungen werden sollen. Die folgende Anforderung gibt beispielsweise Ereignisse für den Benutzer sortiert nach Erstellungsdatum zurück, beginnend mit dem 21. Ereignis in der Sammlung:</span><span class="sxs-lookup"><span data-stu-id="e6bef-p125">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
<span data-ttu-id="e6bef-265">[Ausprobieren im Graph-Tester][skip-example]</span><span class="sxs-lookup"><span data-stu-id="e6bef-265">[Try in Graph Explorer][skip-example]</span></span>

> <span data-ttu-id="e6bef-266">**Hinweis:** Einige Microsoft Graph-APIs, z. B. Outlook-Mail und Outlook-Kalender (**Nachricht**, **Ereignis** und **Kalender**), verwenden `$skip` zur Implementierung von Paging.</span><span class="sxs-lookup"><span data-stu-id="e6bef-266">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (**message**, **event**, and **calendar**), use `$skip` to implement paging.</span></span> <span data-ttu-id="e6bef-267">Wenn Ergebnisse einer Abfrage mehrere Seiten umfassen, geben diese APIs eine `@odata:nextLink`-Eigenschaft mit einer URL zurück, die einen `$skip`-Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="e6bef-267">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="e6bef-268">Sie können diese URL verwenden, um die nächste Seite mit Ergebnissen zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="e6bef-268">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="e6bef-269">Weitere Informationen finden Sie unter [Paging](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="e6bef-269">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="e6bef-270">skipToken-Parameter</span><span class="sxs-lookup"><span data-stu-id="e6bef-270">skipToken parameter</span></span>

<span data-ttu-id="e6bef-p127">Einige Abfragen geben mehrere Seiten von Daten zurück, entweder aufgrund von serverseitigem Paging oder aufgrund der Verwendung des [`$top`](#top-parameter)-Parameters, um die Seitengröße der Antwort zu begrenzen. Viele Microsoft Graph-APIs verwenden den `skipToken`-Abfrageparameter, um auf nachfolgende Seiten des Ergebnisses zu verweisen. Der `$skiptoken`-Parameter enthält ein undurchsichtiges Token, das auf die nächste Seite von Ergebnissen verweist und in der URL zurückgegeben wird, die in der `@odata.nextLink`-Eigenschaft in der Antwort bereitgestellt wird. Weitere Informationen finden Sie unter [Paging](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="e6bef-p127">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top-parameter"></a><span data-ttu-id="e6bef-275">top-Parameter</span><span class="sxs-lookup"><span data-stu-id="e6bef-275">top parameter</span></span>

<span data-ttu-id="e6bef-276">Verwenden Sie den `$top`-Abfrageparameter, um die Seitengröße des Resultsets anzugeben.</span><span class="sxs-lookup"><span data-stu-id="e6bef-276">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="e6bef-277">Wenn mehr Elemente im Resultset verbleiben, enthält der Antworttext einen `@odata.nextLink`-Parameter.</span><span class="sxs-lookup"><span data-stu-id="e6bef-277">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="e6bef-278">Dieser Parameter enthält eine URL, die Sie verwenden können, um die nächste Seite mit Ergebnissen abzurufen.</span><span class="sxs-lookup"><span data-stu-id="e6bef-278">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="e6bef-279">Weitere Informationen finden Sie unter [Paging](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="e6bef-279">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="e6bef-280">Die folgende Anforderung gibt beispielsweise die ersten fünf Nachrichten im Postfach des Benutzers zurück:</span><span class="sxs-lookup"><span data-stu-id="e6bef-280">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<span data-ttu-id="e6bef-281">[Ausprobieren im Graph-Tester][top-example]</span><span class="sxs-lookup"><span data-stu-id="e6bef-281">[Try in Graph Explorer][top-example]</span></span>


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="e6bef-282">Fehlerbehandlung für Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e6bef-282">Error handling for query parameters</span></span>

<span data-ttu-id="e6bef-p129">Einige Anforderungen geben eine Fehlermeldung zurück, wenn ein angegebener Abfrageparameter nicht unterstützt wird. `$expand` kann zum Beispiel nicht in der `user/photo`-Beziehung verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="e6bef-p129">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

```http
https://graph.microsoft.com/beta/me?$expand=photo
```

```json
{
    "error":{
        "code":"ExpandNotSupported",
        "message":"Expand is not allowed for property 'Photo' according to the entity schema.",
        "innerError":{
            "request-id":"1653fefd-bc31-484b-bb10-8dc33cb853ec",
            "date":"2017-07-31T20:55:01"
        }
    }
}
```

<span data-ttu-id="e6bef-285">Beachten Sie jedoch, dass Abfrageparameter, die in einer Anforderung angegeben sind, im Hintergrund einen Fehler verursachen können.</span><span class="sxs-lookup"><span data-stu-id="e6bef-285">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="e6bef-286">Dies gilt für nicht unterstützte Abfrageparameter sowie für nicht unterstützte Kombinationen von Abfrageparametern.</span><span class="sxs-lookup"><span data-stu-id="e6bef-286">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="e6bef-287">In diesen Fällen sollten Sie die von der Anforderung zurückgegebenen Daten überprüfen, um zu ermitteln, ob die angegebenen Abfrageparameter den gewünschten Effekt erzielt haben.</span><span class="sxs-lookup"><span data-stu-id="e6bef-287">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
[count-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0
[expand-example]: https://developer.microsoft.com/graph/graph-explorer?request=groups$expand=members&method=GET&version=v1.0
[filter-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0
[format-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0
[orderby-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0
[search-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0
[select-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0
[skip-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0
[top-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0


