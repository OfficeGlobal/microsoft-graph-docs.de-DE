# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="281a1-101">Verwenden von Abfrageparametern zum Anpassen von Antworten</span><span class="sxs-lookup"><span data-stu-id="281a1-101">Use query parameters to customize responses</span></span>

<span data-ttu-id="281a1-p101">Microsoft Graph stellt optionale Abfrageparameter bereit, die Sie zum Festlegen und Steuern der in einer Antwort zurückgegebenen Datenmenge verwenden können. Die folgenden Abfrageparameter werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="281a1-p101">Microsoft Graph provides optional query parameters that you can use to specify and control the amount of data returned in a response. The following following query parameters are supported.</span></span>

|<span data-ttu-id="281a1-104">Name</span><span class="sxs-lookup"><span data-stu-id="281a1-104">Name</span></span>|<span data-ttu-id="281a1-105">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="281a1-105">Description</span></span>|<span data-ttu-id="281a1-106">Beispiel (klicken Sie auf die Beispiele, um diese im [Graph-Tester][graph-explorer] auszuprobieren)</span><span class="sxs-lookup"><span data-stu-id="281a1-106">Example (click examples to try in [Graph Explorer][graph-explorer])</span></span>
|:---------------|:--------|:-------|
|[<span data-ttu-id="281a1-107">$count</span><span class="sxs-lookup"><span data-stu-id="281a1-107">$count</span></span>](#count)|<span data-ttu-id="281a1-108">Dient zum Abrufen der Gesamtzahl übereinstimmender Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="281a1-108">Retrieves the total count of matching resources.</span></span>|[`/me/messages?$top=2&$count=true`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0)
|[<span data-ttu-id="281a1-109">$expand</span><span class="sxs-lookup"><span data-stu-id="281a1-109">$expand</span></span>](#expand)|<span data-ttu-id="281a1-110">Dient zum Abrufen von verwandten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="281a1-110">Retrieves related resources.</span></span>|[`/groups?$expand=members`](https://developer.microsoft.com/graph/graph-explorer?request=groups$expand=members&method=GET&version=v1.0)
|[<span data-ttu-id="281a1-111">$filter</span><span class="sxs-lookup"><span data-stu-id="281a1-111">$filter</span></span>](#filter)|<span data-ttu-id="281a1-112">Dient zum Filtern von Ergebnissen (Zeilen).</span><span class="sxs-lookup"><span data-stu-id="281a1-112">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)
|[<span data-ttu-id="281a1-113">$orderby</span><span class="sxs-lookup"><span data-stu-id="281a1-113">$orderby</span></span>](#orderby)|<span data-ttu-id="281a1-114">Dient zum Sortieren von Ergebnissen.</span><span class="sxs-lookup"><span data-stu-id="281a1-114">Orders results.</span></span>|[`/users?$orderby=displayName desc`](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0)
|[<span data-ttu-id="281a1-115">$search</span><span class="sxs-lookup"><span data-stu-id="281a1-115">Search</span></span>](#search)| <span data-ttu-id="281a1-p102">Dient zum Zurückgeben von Ergebnissen basierend auf Suchkriterien. Wird derzeit nicht in `messages`- und `person`-Sammlungen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="281a1-p102">Returns results based on search criteria. Currently supported on `messages` and `person` collections.</span></span>|[`/me/messages?$search=pizza`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0)
|[<span data-ttu-id="281a1-118">$select</span><span class="sxs-lookup"><span data-stu-id="281a1-118">$select</span></span>](#select)|<span data-ttu-id="281a1-119">Dient zum Filtern von Eigenschaften (Spalten).</span><span class="sxs-lookup"><span data-stu-id="281a1-119">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`](https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0)
|[<span data-ttu-id="281a1-120">$skip</span><span class="sxs-lookup"><span data-stu-id="281a1-120">$skip</span></span>](#skip)|<span data-ttu-id="281a1-p103">Dient zum Indizieren in einem Resultset. Wird auch von einigen APIs zum Implementieren von Paging verwendet und kann zusammen mit `$top` zum manuellen Auslagern von Ergebnissen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="281a1-p103">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span>  | [`/me/messages?$skip=11`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0)
|[<span data-ttu-id="281a1-123">$skipToken</span><span class="sxs-lookup"><span data-stu-id="281a1-123">$skipToken</span></span>](#skiptoken)|<span data-ttu-id="281a1-p104">Dient zum Abrufen der nächsten Seite von Ergebnissen aus Resultsets, die mehrere Seiten umfassen. (Einige APIs verwenden stattdessen `$skip`.)</span><span class="sxs-lookup"><span data-stu-id="281a1-p104">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `https://graph.microsoft.com/v1.0/users?$skiptoken=X%274453707402000100000017 ... 65612D643839392D343230372D613033662D306332623836633432363932B900000000000000000000%27`
|[<span data-ttu-id="281a1-126">$top</span><span class="sxs-lookup"><span data-stu-id="281a1-126">$top</span></span>](#top)|<span data-ttu-id="281a1-127">Dient zum Festlegen der Seitengröße von Ergebnissen.</span><span class="sxs-lookup"><span data-stu-id="281a1-127">Sets the page size of results.</span></span> |[`/users?$top=2`](https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0)

<span data-ttu-id="281a1-p105">Diese Parameter sind mit der [OData V4-Abfragesprache][odata-query] kompatibel. Nicht alle Parameter werden über alle Microsoft Graph-APIs hinweg unterstützt, und die Unterstützung kann zwischen dem Endpunkt `v1.0` und `beta` erheblich abweichen.</span><span class="sxs-lookup"><span data-stu-id="281a1-p105">These parameters are compatible with the [OData V4 query language][odata-query]. Not all parameters are supported across all Microsoft Graph APIs and support may differ significantly between the `v1.0` and `beta` endpoints.</span></span> 

> <span data-ttu-id="281a1-p106">**Hinweis:** Am `beta`-Endpunkt ist das `$`-Präfix optional. Sie können z. B. `filter` anstelle von `$filter` verwenden. Weitere Informationen und Beispiele finden Sie unter [Abfrageparameter ohne $ Präfixe in Microsoft Graph unterstützen](http://dev.office.com/queryparametersinMicrosoftGraph).</span><span class="sxs-lookup"><span data-stu-id="281a1-p106">**Note:** On the `beta` endpoint, the `$` prefix is optional. For example, instead of `$filter`, you can use `filter`. For more details and examples, see [Supporting query parameters without $ prefixes in Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).</span></span>

<span data-ttu-id="281a1-133">**Codieren von Abfrageparametern:**</span><span class="sxs-lookup"><span data-stu-id="281a1-133">**Encoding query parameters:**</span></span>

<span data-ttu-id="281a1-p107">Die Werte von Abfrageparametern sollten als Prozentwert codiert werden. Viele HTTP-Clients, Browser und Tools (z. B. der [Graph-Tester][graph-explorer]) sind Ihnen dabei behilflich. Wenn eine Abfrage fehlschlägt, kann eine der möglichen Ursachen dafür sein, dass die Werte von Abfrageparametern nicht ordnungsgemäß codiert wurden.</span><span class="sxs-lookup"><span data-stu-id="281a1-p107">The values of query parameters should be percent-encoded. Many HTTP clients, browsers and tools (e.g., the [Graph Explorer][graph-explorer]) will help you with this. If a query is failing, one possible reason is failure to encode the values of query parameters appropriately.</span></span>

<span data-ttu-id="281a1-137">Eine nicht codierte URL sieht folgendermaßen aus:</span><span class="sxs-lookup"><span data-stu-id="281a1-137">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="281a1-138">Eine korrekt codierte URL sieht folgendermaßen aus:</span><span class="sxs-lookup"><span data-stu-id="281a1-138">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count"></a><span data-ttu-id="281a1-139">count</span><span class="sxs-lookup"><span data-stu-id="281a1-139">count</span></span>

<span data-ttu-id="281a1-140">Verwenden Sie `$count` als Abfrageparameter, um die Gesamtzahl der Elemente in einer Sammlung zusammen mit der Seite der Datenwerte anzugeben, die von Microsoft Graph zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="281a1-140">Use `$count` as a query parameter to include a count of the total number of items in a collection alongside the page of data values returned from the Graph, as in the following example:</span></span> 

<span data-ttu-id="281a1-141">Die folgende Anforderung gibt beispielsweise sowohl die `contacts`-Sammlung des aktuellen Benutzers sowie die Anzahl von Elementen in der `contacts`-Sammlung in der `@odata.count`-Eigenschaft zurück.</span><span class="sxs-lookup"><span data-stu-id="281a1-141">For example, the following request will return both the `contacts` collection of the current user, and the number of items in the `contacts` collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="281a1-142">Ausprobieren im Graph-Tester</span><span class="sxs-lookup"><span data-stu-id="281a1-142">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


><span data-ttu-id="281a1-143">**Hinweis:** `$count` wird für Sammlungen von Ressourcen, die von Sammlungen von [Benutzern](../api-reference/v1.0/resources/user.md) oder [Gruppen](../api-reference/v1.0/resources/group.md) abgeleitet werden, die [`directoryObject`](../api-reference/v1.0/resources/directoryobject.md) ähnlich sind, nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="281a1-143">**Note:** `$count` is not supported for collections of resources that derive from [`directoryObject`](../api-reference/v1.0/resources/directoryobject.md) like collections of [user](../api-reference/v1.0/resources/user.md) or [group](../api-reference/v1.0/resources/group.md).</span></span>

## <a name="expand"></a><span data-ttu-id="281a1-144">expand</span><span class="sxs-lookup"><span data-stu-id="281a1-144">expand</span></span>

<span data-ttu-id="281a1-p108">Viele Microsoft Graph-Ressourcen machen sowohl deklarierte Eigenschaften der Ressource sowie deren Beziehungen zu anderen Ressourcen verfügbar. Diese Beziehungen werden auch als Verweiseigenschaften oder Navigationseigenschaften bezeichnet und können auf eine einzelne Ressource oder auf eine Sammlung von Ressourcen verweisen. Beispielsweise werden die E-Mail-Ordner, die Vorgesetzten und die direkten Mitarbeiter eines Benutzers alle als Beziehungen verfügbar gemacht.</span><span class="sxs-lookup"><span data-stu-id="281a1-p108">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources. These relationships are also called reference properties or navigation properties and they can reference either a single resource or a collection of resources. For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="281a1-p109">Normalerweise können Sie die Eigenschaften einer Ressource oder eine ihrer Beziehungen in einer einzelnen Anforderung abfragen, aber nicht beides gleichzeitig. Sie können den `$expand`-Zeichenfolgen-Abfrageparameter verwenden, um die erweiterte Ressource oder die Sammlung, auf die von einer einzigen Beziehung verwiesen wird (Navigationseigenschaft) in Ihre Ergebnisse einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="281a1-p109">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="281a1-150">Im folgenden Beispiel werden Informationen des Stammlaufwerks zusammen mit den untergeordneten Elementen der obersten Ebene in einem Laufwerk abgerufen:</span><span class="sxs-lookup"><span data-stu-id="281a1-150">The following example gets root drive information along with the top level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="281a1-151">Ausprobieren im Graph-Tester</span><span class="sxs-lookup"><span data-stu-id="281a1-151">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="281a1-p110">Bei einigen Ressourcensammlungen können Sie auch die Eigenschaften angeben, die in den erweiterten Ressourcen zurückgegeben werden sollen, indem Sie einen `$select`-Parameter hinzufügen. Im folgenden Beispiel wird die gleiche Abfrage wie im vorherigen Beispiel ausgeführt, hier wird jedoch eine [`$select`](#select)-Anweisung verwendet, um die für die erweiterten untergeordneten Element zurückgegebenen Eigenschaften auf die Eigenschaften `id` und `name` zu beschränken.</span><span class="sxs-lookup"><span data-stu-id="281a1-p110">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select) statement to limit the properties returned for the expanded child items to the `id` and `name` properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="281a1-154">[Ausprobieren im Graph-Tester](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children($select=id,name)&method=GET&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="281a1-154">[Try in Graph Explorer](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children($select=id,name)&method=GET&version=v1.0)</span></span>

> <span data-ttu-id="281a1-p111">**Hinweis:** Nicht alle Beziehungen und Ressourcen unterstützen den `$expand`-Abfrageparameter. Sie können z. B. die Beziehungen `directReports`, `manager` und `memberOf` für einen Benutzer erweitern, aber Sie können nicht seine Beziehungen `events`, `messages` oder `photo` erweitern. Nicht alle Ressourcen oder Beziehungen unterstützen die Verwendung von `$select` in erweiterten Elementen.</span><span class="sxs-lookup"><span data-stu-id="281a1-p111">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the `directReports`, `manager`, and `memberOf` relationships on a user, but you cannot expand its `events`, `messages`, or `photo` relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="281a1-158">Bei Azure AD-Ressourcen, die von [directoryObject](../api-reference/v1.0/resources/directoryobject.md) abgeleitet werden, z. B. [Benutzer](../api-reference/v1.0/resources/user.md) und [Gruppe](../api-reference/v1.0/resources/group.md), wird `$expand` nur für `beta` unterstützt, und es werden maximal 20 Elemente für die erweiterte Beziehung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="281a1-158">With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter"></a><span data-ttu-id="281a1-159">Filter</span><span class="sxs-lookup"><span data-stu-id="281a1-159">filter</span></span>

<span data-ttu-id="281a1-160">Verwenden Sie den `$filter`-Abfrageparameter, um nur eine Teilmenge einer Sammlung abzurufen.</span><span class="sxs-lookup"><span data-stu-id="281a1-160">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> 

<span data-ttu-id="281a1-161">Um beispielsweise Benutzer zu suchen, deren Anzeigename mit dem Buchstaben „J“ beginnt, verwenden Sie `startswith`.</span><span class="sxs-lookup"><span data-stu-id="281a1-161">For example, to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="281a1-162">[Ausprobieren im Graph-Tester](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="281a1-162">[Try in Graph Explorer](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)</span></span>

<span data-ttu-id="281a1-p112">Die Unterstützung für `$filter`-Operatoren variiert je nach Microsoft Graph-APIs. Die folgenden logischen Operatoren werden im Allgemeinen unterstützt: gleich (`eq`), ungleich (`ne`), größer als (`gt`), größer als oder gleich (`ge`), kleiner als (`lt`), kleiner als oder gleich (`le`), und (`and`), oder (`or`), und nicht (`not`). Der `startswith`-Zeichenfolgenoperator wird häufig unterstützt. Der `any`- Lambda-Operator wird für einige APIs unterstützt. In der folgenden Tabelle finden Sie einige Verwendungsbeispiele. Weitere Informationen zur `$filter`-Syntax finden Sie im [OData-Protokoll][odata-filter].</span><span class="sxs-lookup"><span data-stu-id="281a1-p112">Support for `$filter` operators varies across Microsoft Graph APIs. The following logical operators are generally supported: equals (`eq`), not equals (`ne`), greater than (`gt`), greater than or equals (`ge`), less than (`lt`), less than or equals (`le`), and (`and`), or (`or`), and not (`not`). The `startswith` string operator is often supported. The `any` lambda operator is supported for some APIs. For some  usage examples, see the table below. For additional details on `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="281a1-169">Die folgende Tabelle enthält einige Beispiele zur Verwendung des `$filter`-Abfrageparameters.</span><span class="sxs-lookup"><span data-stu-id="281a1-169">The following table shows some examples using the `$filter` query parameter.</span></span>

|<span data-ttu-id="281a1-170">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="281a1-170">Description</span></span>|<span data-ttu-id="281a1-171">Beispiel (klicken Sie auf die Beispiele, um diese im [Graph-Tester][graph-explorer] auszuprobieren)</span><span class="sxs-lookup"><span data-stu-id="281a1-171">Example (click examples to try in [Graph Explorer][graph-explorer])</span></span>|
|:--------|:-------|
|  <span data-ttu-id="281a1-172">Suchen Sie nach Benutzern mit dem Namen „Mary“ über mehrere Eigenschaften hinweg.</span><span class="sxs-lookup"><span data-stu-id="281a1-172">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) |
| <span data-ttu-id="281a1-173">Rufen Sie alle Ereignisse des angemeldeten Benutzers ab, die nach dem 01.07.2017 beginnen.</span><span class="sxs-lookup"><span data-stu-id="281a1-173">Get all of the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) |
| <span data-ttu-id="281a1-174">Rufen Sie alle E-Mails von einer bestimmten Adresse ab, die der angemeldete Benutzer erhalten hat.</span><span class="sxs-lookup"><span data-stu-id="281a1-174">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) |
| <span data-ttu-id="281a1-175">Rufen Sie alle E-Mail ab, die der angemeldete Benutzer im April 2017 erhalten hat.</span><span class="sxs-lookup"><span data-stu-id="281a1-175">Get all emails received by the signed-in user in April 2017</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) |
| <span data-ttu-id="281a1-176">Rufen Sie alle ungelesenen E-Mails im Postfach des angemeldeten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="281a1-176">Get all unread mails in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) |
| <span data-ttu-id="281a1-177">Auflisten aller Office 365-Gruppen in einer Organisation</span><span class="sxs-lookup"><span data-stu-id="281a1-177">List all Office 365 groups in an organization</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) |

> <span data-ttu-id="281a1-p113">**Hinweis:** Die folgenden `$filter`-Operatoren werden für Azure AD-Ressourcen nicht unterstützt: `ne`, `gt`, `ge`, `lt`, `le` und `not`. Der `contains`-Zeichenfolgenoperator wird derzeit nicht für Microsoft Graph-Ressourcen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="281a1-p113">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="orderby"></a><span data-ttu-id="281a1-180">orderby</span><span class="sxs-lookup"><span data-stu-id="281a1-180">orderby</span></span>

<span data-ttu-id="281a1-181">Verwenden Sie zum Festlegen der Sortierreihenfolge der von Microsoft Graph zurückgegebenen Elemente den `$orderby`-Abfrageparameter.</span><span class="sxs-lookup"><span data-stu-id="281a1-181">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="281a1-182">Die folgende Anforderung gibt beispielsweise die Benutzer in der Organisation sortiert nach ihrem Anzeigenamen zurück:</span><span class="sxs-lookup"><span data-stu-id="281a1-182">For example, to return the users in the organization ordered by their display name, the syntax is as follows:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
[<span data-ttu-id="281a1-183">Ausprobieren im Graph-Tester</span><span class="sxs-lookup"><span data-stu-id="281a1-183">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName&method=GET&version=v1.0)

<span data-ttu-id="281a1-p114">Sie können auch nach komplexen Typentitäten sortieren. In der folgenden Anforderungen werden Nachrichten abgerufen und nach dem `address`-Feld der `from`-Eigenschaft sortiert, die vom komplexen Typ `emailAddress` ist:</span><span class="sxs-lookup"><span data-stu-id="281a1-p114">You can also sort by complex type entities. The following example gets messages and sorts them by the `address` field of the `from` property, which is of the complex type `emailAddress`:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="281a1-186">Ausprobieren im Graph-Tester</span><span class="sxs-lookup"><span data-stu-id="281a1-186">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="281a1-187">Wenn Sie die Ergebnisse in aufsteigender oder absteigender Reihenfolge sortieren möchten, fügen Sie entweder `asc` oder `desc` an den Namen des Felds getrennt durch ein Leerzeichen an, z. B. `?$orderby=name%20desc`.</span><span class="sxs-lookup"><span data-stu-id="281a1-187">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space, for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="281a1-p115">Bei einigen APIs können Sie die Ergebnisse anhand mehrerer Eigenschaften sortieren. Die folgende Anforderung sortiert die Nachrichten im Posteingang des Benutzers beispielsweise zuerst nach dem Namen der Person, die die Nachricht gesendet hat, in absteigender Reihenfolge (von Z nach A) und anschließend nach dem Betreff in aufsteigender Reihenfolge (Standard).</span><span class="sxs-lookup"><span data-stu-id="281a1-p115">With some APIs, you can order results on multiple properties. For example, the following request orders the messages in the user's Inbox first by the name of the person who sent it in descending order (Z to A) and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```
[<span data-ttu-id="281a1-190">Ausprobieren im Graph-Tester</span><span class="sxs-lookup"><span data-stu-id="281a1-190">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)


 > <span data-ttu-id="281a1-191">**Hinweis:** Bei Azure AD-Ressourcen, die von [directoryObject](../api-reference/v1.0/resources/directoryobject.md) abgeleitet werden, wie z. B. [Benutzer](../api-reference/v1.0/resources/user.md) und [Gruppe](../api-reference/v1.0/resources/group.md), kann `$orderby` nicht mit `$filter`-Ausdrücken verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="281a1-191">**Note:** With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search"></a><span data-ttu-id="281a1-192">Suche</span><span class="sxs-lookup"><span data-stu-id="281a1-192">search</span></span>

<span data-ttu-id="281a1-193">Um die Ergebnisse einer Anforderung so zu beschränken, dass sie einem Suchkriterium entsprechen, verwenden Sie den `$search`-Abfrageparameter.</span><span class="sxs-lookup"><span data-stu-id="281a1-193">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

> <span data-ttu-id="281a1-p116">**Hinweis:** Sie können derzeit **nur** [Nachrichten](../api-reference/v1.0/resources/message.md)- und [Personen](../api-reference/v1.0/resources/person.md)-Sammlungen suchen. Eine `$search`-Anforderung gibt bis zu 250 Ergebnisse zurück. Sie können [`$filter`](#filter) oder [`$orderby`](#orderby) nicht in einer Suchabfrage verwenden.</span><span class="sxs-lookup"><span data-stu-id="281a1-p116">**Note:** You can currently **only** search [message](../api-reference/v1.0/resources/message.md) and [person](../api-reference/v1.0/resources/person.md) collections. A `$search` request returns up to 250 results. You cannot use [`$filter`](#filter) or [`$orderby`](#orderby) in a search request.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="281a1-197">Verwenden von $search in `message`-Sammlungen</span><span class="sxs-lookup"><span data-stu-id="281a1-197">Using $search on `message` collections</span></span>

<span data-ttu-id="281a1-p117">Suchkriterien für Nachrichten werden mithilfe von [Advanced Query Syntax (AQS)](https://support.office.com/article/Search-Mail-and-People-in-Outlook-com-and-Outlook-on-the-web-for-business-88108edf-028e-4306-b87e-7400bbb40aa7) ausgedrückt. Die Ergebnisse sind nach Datum und Uhrzeit sortiert, zu dem bzw. der die Nachricht gesendet wurde.</span><span class="sxs-lookup"><span data-stu-id="281a1-p117">Search criteria are expressed using Advanced Query Syntax (AQS). The results are sorted by the date and time that the message was sent.</span></span>

<span data-ttu-id="281a1-200">Sie können die folgenden Eigenschaften in einer `message` in einem `$search`-Kriterium angeben: `attachments`, `bccRecipients`, `body`, `category`, `ccRecipients`, `content`, `from`, `hasAttachments`, `participants`, `receivedDateTime`, `sender`, `subject`,`toRecipients`</span><span class="sxs-lookup"><span data-stu-id="281a1-200">You can specify the following properties on a `message` in a `$search` criterion: `attachments`, `bccRecipients`, `body`, `category`, `ccRecipients`, `content`, `from`, `hasAttachments`, `participants`, `receivedDateTime`, `sender`, `subject`, `toRecipients`</span></span>

<span data-ttu-id="281a1-201">Wenn Sie eine Suche nach Nachrichten durchführen und nur einen Wert angeben, wird die Suche anhand der Standardsucheigenschaften`from`, `subject` und `body` ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="281a1-201">If you do a search on messages and specify only a value, the search is carried out on the default search properties of `from`, `subject` and `body`.</span></span>

<span data-ttu-id="281a1-202">Im folgenden Beispiel werden alle Nachrichten im Posteingang des angemeldeten Benutzers zurückgegeben, die das Wort „Pizza“ in einer der drei Standardsucheigenschaften enthalten:</span><span class="sxs-lookup"><span data-stu-id="281a1-202">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="281a1-203">Im nächsten Beispiel werden alle Nachrichten im Posteingang des Benutzers, die von einer bestimmten E-Mail-Adresse gesendet wurden:</span><span class="sxs-lookup"><span data-stu-id="281a1-203">The next example searches all messages in the user's Inbox that were sent from a specific email address:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

### <a name="using-search-on-person-collections"></a><span data-ttu-id="281a1-204">Verwenden von $search in `person`-Sammlungen</span><span class="sxs-lookup"><span data-stu-id="281a1-204">Using $search on `person` collections</span></span>

<span data-ttu-id="281a1-p118">Sie können die Personen-API von Microsoft Graph verwenden, um Personen abzurufen, die für einen Benutzer am relevantesten sind. Relevanz wird durch die Kommunikations- und Zusammenarbeitsmuster und Geschäftsbeziehungen des Benutzers bestimmt. Die Personen-API unterstützt den `$search`-Abfrageparameter.</span><span class="sxs-lookup"><span data-stu-id="281a1-p118">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. The People API supports the `$search` query parameter.</span></span>

<span data-ttu-id="281a1-p119">Personensuchen werden sowohl für die Eigenschaft `displayName` als auch für die Eigenschaft `emailAddress`der [Person](../api-reference/v1.0/resources/person.md) ausgeführt. Suchvorgänge implementieren einen Algorithmus für Fuzzyübereinstimmungen. Dabei werden Ergebnisse basierend auf einer exakten Übereinstimmung und auch zu Rückschlüssen zu der Absicht der Suche zurückgegeben. Verwenden wir als Beispiel einen Benutzer mit dem Anzeigenamen „Tyler Lee“ und der E-Mail-Adresse „tylerle@example.com“, der sich in der `people`-Sammlung des angemeldeten Benutzers befindet. Bei allen der folgenden Suchvorgänge werden Ergebnisse zurückgegeben, die „Tyler“ enthalten.</span><span class="sxs-lookup"><span data-stu-id="281a1-p119">Searches on people occur on both the `displayName` and `emailAddress` properties of the [person](../api-reference/v1.0/resources/person.md) resource. Searches implement a fuzzy matching algorithm. They will return results based on an exact match and also on inferences about the intent of the search. For example, imagine a user with a display name of "Tyler Lee" and an email address of tylerle@example.com who is in the `people` collection of the signed-in user. All of the following searches will return results that contain Tyler.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people?$search=tyler                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search=tylerle              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search=tiler                //fuzzy match with Tyler's name 
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"          //matches Tyler's name. Note the quotes to enclose the space.
```

<span data-ttu-id="281a1-p120">Sie können Suchen nach Personen durchführen, die an einem bestimmten Thema interessiert sind. Suchvorgänge werden basierend auf Rückschlüssen ausgeführt, die aus den E-Mail-Unterhaltungen des Benutzers abgeleitet werden. Die folgende Suche gibt beispielsweise eine Sammlung von Personen zurück, die für den angemeldeten Benutzer relevant sind und in Unterhaltungen mit diesem Benutzer Interesse an Pizza geäußert haben. Beachten Sie, dass der Suchbegriff in Anführungszeichen eingeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="281a1-p120">You can also perform searches for people who are interested in a particular topic. Searches are performed based on inferences derived from the user's mail conversations. For example, the following search will return a collection of people relevant to the signed-in user who have expressed an interest in pizza in communications with that user. Note that the search phrase is enclosed in quotes.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:pizza"                
```

<span data-ttu-id="281a1-217">Sie können auch Personen- und Themensuchen in derselben Anforderung kombinieren, indem Sie die beiden Typen von Suchausdrücken kombinieren.</span><span class="sxs-lookup"><span data-stu-id="281a1-217">Finally, you can combine both people searches and topic searches in the same request by combining the two types of search expression.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="tyl topic:pizza"                
```
<span data-ttu-id="281a1-p121">Bei dieser Anforderung werden im Wesentlichen zwei Suchvorgänge ausgeführt: eine unscharfe Suche in den Eigenschaften `displayName` und `emailAddress` der relevanten Personen des angemeldeten Benutzers und eine Themensuche nach „Pizza“ in den relevanten Personen des Benutzers. Die Ergebnisse sind dann bewertet, sortiert und zurückgegeben. Beachten Sie, dass die Suche nicht restriktiv ist. Sie erhalten möglicherweise Ergebnisse, die Personen enthalten, die mit „tyl“ übereinstimmen oder die an „Pizza“ interessiert sind oder beides.</span><span class="sxs-lookup"><span data-stu-id="281a1-p121">This request essentially conducts two searches: a fuzzy search against `displayName` and `emailAddress` properties of the signed-in user's relevant people and a topic search for "pizza" against the user's relevant people. The results are then ranked, ordered, and returned. Note that the search is not restrictive; you may get results that contain people that fuzzy match "tyl", or that are interested in "pizza", or both.</span></span>

<span data-ttu-id="281a1-221">Weitere Informationen zur Personen-API finden Sie unter [Abrufen von Informationen über die entsprechenden Personen](./people_example.md).</span><span class="sxs-lookup"><span data-stu-id="281a1-221">To learn more about the People API, see [Get information about relevant people](./people_example.md).</span></span>  

## <a name="select"></a><span data-ttu-id="281a1-222">select</span><span class="sxs-lookup"><span data-stu-id="281a1-222">select</span></span>

<span data-ttu-id="281a1-p122">Verwenden Sie den `$select`-Abfrageparameter, um eine Reihe von Eigenschaften zurückzugeben, die sich von den Standardeigenschaften für eine einzelne Ressource oder eine Sammlung von Ressourcen unterscheidet. Mit $select können Sie eine Teilmenge oder eine Obermenge der Standardeigenschaften angeben.</span><span class="sxs-lookup"><span data-stu-id="281a1-p122">Use the `$select` query parameter to return a set of properties different than the default set for an individual resource or a collection of resources. With $select you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="281a1-225">Wenn Sie z. B. die Nachrichten des angemeldeten Benutzers abrufen, können Sie angeben, dass nur die Eigenschaften `from` und `subject` zurückgegeben werden:</span><span class="sxs-lookup"><span data-stu-id="281a1-225">For example, when retrieving the messages of the signed-in user, you can specify that only the `from` and `subject` properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

[<span data-ttu-id="281a1-226">Ausprobieren im Graph-Tester</span><span class="sxs-lookup"><span data-stu-id="281a1-226">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$select=from,subject&method=GET&version=v1.0)

> <span data-ttu-id="281a1-p123">**Wichtig:** Im Allgemeinen wird empfohlen, dass Sie `$select` verwenden, um die von einer Abfrage zurückgegebenen Eigenschaften auf diejenigen zu beschränken, die von Ihrer App benötigt werden. Dies gilt insbesondere für Abfragen, die möglicherweise ein großes Resultset zurückgeben. Durch Beschränken der in jeder Zeile zurückgegebenen Eigenschaften wird die Netzwerklast reduziert und die Leistung Ihrer App verbessert.</span><span class="sxs-lookup"><span data-stu-id="281a1-p123">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app. This is especially true of queries that may potentially return a large result set. Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="281a1-p124">In `v1.0` geben einige Azure AD-Ressourcen, die von [directoryObject](../api-reference/v1.0/resources/directoryobject.md) abgeleitet werden, z.B. [Benutzer](../api-reference/v1.0/resources/user.md) und [Gruppe](../api-reference/v1.0/resources/group.md) eine begrenzte, standardmäßige Untermenge von Eigenschaften für Lesevorgänge zurück. Für diese Ressourcen müssen Sie `$select` verwenden, um Eigenschaften außerhalb des Standardsatzes zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="281a1-p124">In `v1.0`, some Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip"></a><span data-ttu-id="281a1-232">skip</span><span class="sxs-lookup"><span data-stu-id="281a1-232">skip</span></span>

<span data-ttu-id="281a1-p125">Verwenden Sie den `$skip`-Abfrageparameter zum Festlegen der Anzahl der Elemente, die am Anfang einer Sammlung übersprungen werden sollen. Die folgende Anforderung gibt beispielsweise Ereignisse für den Benutzer sortiert nach Erstellungsdatum zurück, beginnend mit dem 21. Ereignis in der Sammlung:</span><span class="sxs-lookup"><span data-stu-id="281a1-p125">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
[<span data-ttu-id="281a1-235">Ausprobieren im Graph-Tester</span><span class="sxs-lookup"><span data-stu-id="281a1-235">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$orderby=createdDateTime&$skip=20&method=GET&version=v1.0)

> <span data-ttu-id="281a1-p126">**Hinweis:** Einige Microsoft Graph-APIs, z. B. Outlook E-Mail und Kalender (`message`, `event` und `calendar`), verwenden `$skip` zur Implementierung von Paging. Wenn Ergebnisse einer Abfrage mehrere Seiten umfassen, geben diese APIs eine `@odata:nextLink`-Eigenschaft mit einer URL zurück, die einen `$skip`-Parameter enthält. Sie können diese URL verwenden, um die nächste Seite von Ergebnissen zurückzugeben. Weitere Informationen finden Sie unter [Paging](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="281a1-p126">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (`message`, `event`, and, `calendar`), use `$skip` to implement paging. When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter. You can use this URL to return the next page of results. To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken"></a><span data-ttu-id="281a1-240">skipToken</span><span class="sxs-lookup"><span data-stu-id="281a1-240">skipToken</span></span>

<span data-ttu-id="281a1-p127">Einige Abfragen geben mehrere Seiten von Daten zurück, entweder aufgrund von serverseitigem Paging oder aufgrund der Verwendung des [`$top`](#top)-Parameters, um die Seitengröße der Antwort zu begrenzen. Viele Microsoft Graph-APIs verwenden den `skipToken`-Abfrageparameter, um auf nachfolgende Seiten des Ergebnisses zu verweisen. Der `$skiptoken`-Parameter enthält ein undurchsichtiges Token, das auf die nächste Seite von Ergebnissen verweist und in der URL zurückgegeben wird, die in der `@odata.nextLink`-Eigenschaft in der Antwort bereitgestellt wird. Weitere Informationen finden Sie unter [Paging](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="281a1-p127">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top"></a><span data-ttu-id="281a1-245">top</span><span class="sxs-lookup"><span data-stu-id="281a1-245">top</span></span>

<span data-ttu-id="281a1-246">Verwenden Sie den `$top`-Abfrageparameter, um die Seitengröße des Resultsets anzugeben.</span><span class="sxs-lookup"><span data-stu-id="281a1-246">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="281a1-p128">Wenn es weitere Elemente gibt, die im Resultset verbleiben, enthält der Antworttext einen `@odata.nextLink`-Parameter. Dieser Parameter enthält eine URL, die Sie verwenden können, um die nächste Seite von Ergebnissen abzurufen. Weitere Informationen finden Sie unter [Paging](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="281a1-p128">If there are more items remaining in the result set, the response body will contain an `@odata.nextLink` parameter. This parameter contains a URL that you can use to get the next page of results. To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="281a1-250">Die folgende Anforderung gibt beispielsweise die ersten fünf Nachrichten im Postfach des Benutzers zurück:</span><span class="sxs-lookup"><span data-stu-id="281a1-250">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

[<span data-ttu-id="281a1-251">Ausprobieren im Graph-Tester</span><span class="sxs-lookup"><span data-stu-id="281a1-251">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=5&method=GET&version=v1.0)


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="281a1-252">Fehlerbehandlung für Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="281a1-252">Error handling for query parameters</span></span>

<span data-ttu-id="281a1-p129">Einige Anforderungen geben eine Fehlermeldung zurück, wenn ein angegebener Abfrageparameter nicht unterstützt wird. `$expand` kann zum Beispiel nicht in der `user/photo`-Beziehung verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="281a1-p129">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

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

<span data-ttu-id="281a1-p130">Beachten Sie jedoch, dass Abfrageparameter, die in einer Anforderung angegeben sind, im Hintergrund einen Fehler verursachen. Dies gilt für nicht unterstützte Abfrageparameter sowie für nicht unterstützte Kombinationen von Abfrageparametern. In diesen Fällen sollten Sie die von der Anforderung zurückgegebenen Daten überprüfen, um zu ermitteln, ob die angegebenen Abfrageparameter den gewünschten Effekt erzielt haben.</span><span class="sxs-lookup"><span data-stu-id="281a1-p130">However, it is important to note that query parameters specified in a request may fail silently. This can be true for unsupported query parameters as well as for unsupported combinations of query parameters. In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356