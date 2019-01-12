---
title: 'Paging der Microsoft Graph-Daten in Ihrer App '
description: 'odata.nextLink-Eigenschaft in der Antwort, die eine URL zur nächsten Seite mit Ergebnissen enthält. '
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 6a19d1873057f5a6f6ea1749a6941389b9be8eb5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830660"
---
# <a name="paging-microsoft-graph-data-in-your-app"></a><span data-ttu-id="39eac-103">Paging der Microsoft Graph-Daten in Ihrer App</span><span class="sxs-lookup"><span data-stu-id="39eac-103">Paging Microsoft Graph data in your app</span></span> 

<span data-ttu-id="39eac-p101">Einige Abfragen in Microsoft Graph geben mehrere Seiten von Daten zurück, entweder aufgrund von serverseitigem Paging oder aufgrund der Verwendung des `$top`-Abfrageparameters, um die Seitengröße in einer Anforderung gezielt zu begrenzen. Wenn ein Resultset mehrere Seiten umfasst, gibt Microsoft Graph eine `@odata.nextLink`-Eigenschaft in der Antwort, die eine URL zu der nächsten Seite mit Ergebnissen enthält.</span><span class="sxs-lookup"><span data-stu-id="39eac-p101">Some queries against Microsoft Graph return multiple pages of data either due to server-side paging or due to the use of the `$top` query parameter to specifically limit the page size in a request. When a result set spans multiple pages, Microsoft Graph returns an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> 

<span data-ttu-id="39eac-106">Die folgende URL fordert beispielsweise alle Benutzer in einer Organisation mit einer Seitengröße von 5 an, die mit dem `$top`-Abfrageparameter angegeben wird:</span><span class="sxs-lookup"><span data-stu-id="39eac-106">For example, the following URL requests all the users in an organization with a page size of 5, specified with the `$top` query parameter:</span></span>

```html
https://graph.microsoft.com/v1.0/users?$top=5
```

<span data-ttu-id="39eac-107">Wenn das Ergebnis mehr als fünf Benutzer enthält, gibt Microsoft Graph eine `@odata:nextLink`-Eigenschaft ähnlich der folgenden zusammen mit der ersten Seite von Benutzern zurück.</span><span class="sxs-lookup"><span data-stu-id="39eac-107">If the result contains more than five users, Microsoft Graph will return an `@odata:nextLink` property similar to the following along with the first page of users.</span></span>

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27"
```

<span data-ttu-id="39eac-108">Sie können die nächste Seite mit Ergebnissen abrufen, indem Sie den URL-Wert der `@odata:nextLink`-Eigenschaft an Microsoft Graph senden.</span><span class="sxs-lookup"><span data-stu-id="39eac-108">You can retrieve the next page of results by sending the URL value of the `@odata:nextLink` property to Microsoft Graph.</span></span> 

```html
https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27
```

<span data-ttu-id="39eac-109">Microsoft Graph gibt weiterhin einen Verweis auf die nächste Seite von Daten in der `@odata:nextLink`-Eigenschaft mit jeder Antwort zurück, bis alle Seiten des Ergebnisses gelesen wurden.</span><span class="sxs-lookup"><span data-stu-id="39eac-109">Microsoft Graph will continue to return a reference to the next page of data in the `@odata:nextLink` property with each response until all pages of the result have been read.</span></span>

><span data-ttu-id="39eac-110">**Wichtig:** Sie sollten die gesamte URL in die `@odata:nextLink`-Eigenschaft in Ihrer Anforderung für die nächste Seite mit Ergebnissen einschließen.</span><span class="sxs-lookup"><span data-stu-id="39eac-110">**Important:** You should include the entire URL in the `@odata:nextLink` property in your request for the next page of results.</span></span> <span data-ttu-id="39eac-111">In Abhängigkeit von der API, für die die Abfrage ausgeführt wird, enthält der `@odata:nextLink`-URL-Wert entweder den Abfrageparameter `$skiptoken` oder `$skip`.</span><span class="sxs-lookup"><span data-stu-id="39eac-111">Depending on the API that the query is being performed against, the `@odata:nextLink` URL value will contain either a `$skiptoken` or a `$skip` query parameter.</span></span> <span data-ttu-id="39eac-112">Die URL enthält auch alle anderen Abfrageparameter, die in der ursprünglichen Anforderung vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="39eac-112">The URL also contains all the other query parameters present in the original request.</span></span> <span data-ttu-id="39eac-113">Versuchen Sie nicht, den Wert von `$skiptoken` oder `$skip` zu extrahieren und in einer anderen Anforderung zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="39eac-113">Do not try to extract the `$skiptoken` or `$skip` value and use it in a different request.</span></span> 

<span data-ttu-id="39eac-114">Das Paging-Verhalten variiert in den verschiedenen Microsoft Graph-APIs.</span><span class="sxs-lookup"><span data-stu-id="39eac-114">Paging behavior varies across different Microsoft Graph APIs.</span></span> <span data-ttu-id="39eac-115">Berücksichtigen Sie beim Arbeiten mit ausgelagerten Daten die folgenden Punkte:</span><span class="sxs-lookup"><span data-stu-id="39eac-115">Consider the following when working with paged data:</span></span>

- <span data-ttu-id="39eac-116">Unterschiedliche APIs weisen möglicherweise unterschiedliche Standard- und Maximalgrößen für Seiten auf.</span><span class="sxs-lookup"><span data-stu-id="39eac-116">Different APIs might have different default and maximum page sizes.</span></span>
- <span data-ttu-id="39eac-117">Unterschiedliche APIs verhalten sich möglicherweise unterschiedlich, wenn Sie eine Seitengröße (über den `$top`-Abfrageparameter) angeben, der die maximale Seitengröße für diese API überschreitet.</span><span class="sxs-lookup"><span data-stu-id="39eac-117">Different APIs might behave differently if you specify a page size (via the `$top` query parameter) that exceeds the maximum page size for that API.</span></span> <span data-ttu-id="39eac-118">Je nach API wird die angeforderte Seitengröße möglicherweise ignoriert oder standardmäßig auf die maximale Seitengröße für diese API festgelegt, oder Microsoft Graph gibt einen Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="39eac-118">Depending on the API, the requested page size might be ignored, it might default to the maximum page size for that API, or Microsoft Graph might return an error.</span></span> 
- <span data-ttu-id="39eac-p105">Nicht alle Ressourcen oder Beziehungen unterstützen Paging. Abfragen von [directoryRoles](/graph/api/resources/directoryrole?view=graph-rest-1.0) unterstützen beispielsweise kein Paging. Dies umfasst das Lesen von Rollenobjekten und Rollenmitgliedern.</span><span class="sxs-lookup"><span data-stu-id="39eac-p105">Not all resources or relationships support paging. For example, queries against [directoryRoles](/graph/api/resources/directoryrole?view=graph-rest-1.0) do not support paging. This includes reading role objects themselves as well as role members.</span></span>
