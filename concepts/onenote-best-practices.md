---
title: Bewährte Methoden für die Arbeit mit OneNote-APIs in Microsoft Graph.
description: Dieser Artikel enthält Vorschläge für die Arbeit mit OneNote-APIs in Microsoft Graph. Diese Empfehlungen basieren auf den Antworten auf häufig gestellte Fragen auf Stack Overflow und Twitter.
author: Jewan-microsoft
ms.openlocfilehash: f02976424ea39935e38d45b7eb2f80ba66319c7e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332165"
---
# <a name="best-practices-for-working-with-the-onenote-api-in-microsoft-graph"></a><span data-ttu-id="7a901-104">Bewährte Methoden für die Arbeit mit OneNote-APIs in Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7a901-104">Best practices for working with the OneNote API in Microsoft Graph</span></span>

<span data-ttu-id="7a901-105">Dieser Artikel enthält Vorschläge für die Arbeit mit OneNote-APIs in Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7a901-105">This article provides recommendations for working with the OneNote APIs in Microsoft Graph.</span></span> <span data-ttu-id="7a901-106">Diese Empfehlungen basieren auf den Antworten auf häufig gestellte Fragen auf Stack Overflow und Twitter.</span><span class="sxs-lookup"><span data-stu-id="7a901-106">These recommendations are based on answers to common questions on Stack Overflow and Twitter.</span></span>

## <a name="use-select-to-select-the-minimum-set-of-properties-you-need"></a><span data-ttu-id="7a901-107">Verwenden von $select, um die minimale Anzahl der benötigten Eigenschaften auszuwählen</span><span class="sxs-lookup"><span data-stu-id="7a901-107">Use $select to select the minimum set of properties you need</span></span>

<span data-ttu-id="7a901-108">Wenn Sie eine Ressource (z. B. Abschnitte innerhalb eines Notizbuchs) abfragen, verwende Sie eine ähnliche Abfrage wie die folgende.</span><span class="sxs-lookup"><span data-stu-id="7a901-108">When you query for a resource (for example, sections inside a notebook), you make a request similar to the following.</span></span>

```http
GET ~/notebooks/{id}/sections
```

<span data-ttu-id="7a901-109">Es werden alle Eigenschaften der Abschnitte abgerufen.</span><span class="sxs-lookup"><span data-stu-id="7a901-109">This retrieves all the properties of the sections.</span></span> <span data-ttu-id="7a901-110">Allerdings benötigen Sie möglicherweise nicht alle Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="7a901-110">However, you might not need all properties.</span></span> <span data-ttu-id="7a901-111">Sie können den `$select`-Abfragenparameter verwenden, um nur die gewünschten, Eigenschaften zurückzugeben, wie im folgenden Beispiel gezeigt.</span><span class="sxs-lookup"><span data-stu-id="7a901-111">You can use the `$select` query parameter to return just the properties that you want, as shown in the following example.</span></span>

```http
GET ~/notebooks/{id}/sections?$select=id,displayName
```

<span data-ttu-id="7a901-112">Der gleiche Ansatz gilt für andere OneNote-APIs.</span><span class="sxs-lookup"><span data-stu-id="7a901-112">The same approach applies to other OneNote APIs.</span></span>

## <a name="use-expand-instead-of-making-multiple-api-calls"></a><span data-ttu-id="7a901-113">Verwenden von $expand, anstatt mehrere API-Aufrufe auszuführen</span><span class="sxs-lookup"><span data-stu-id="7a901-113">Use $expand instead of making multiple API calls</span></span>

<span data-ttu-id="7a901-114">Nehmen wir an, dass Sie alle Notizbücher, Abschnitte und Abschnittsgruppen des Benutzers in einer hierarchischen Ansicht abrufen möchten.</span><span class="sxs-lookup"><span data-stu-id="7a901-114">Suppose you want to retrieve all of the user’s notebooks, sections, and section groups in a hierarchical view.</span></span> <span data-ttu-id="7a901-115">Dazu können Sie folgendermaßen vorgehen:</span><span class="sxs-lookup"><span data-stu-id="7a901-115">You might accomplish that by doing the following:</span></span>

* <span data-ttu-id="7a901-116">Rufen Sie `GET ~/notebooks` auf, um die Liste der Notizbücher anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="7a901-116">Call `GET ~/notebooks` to get the list of notebooks.</span></span>

* <span data-ttu-id="7a901-117">Rufen Sie für jedes abgerufene Notizbuch `GET ~/notebooks/{notebookId}/sections` auf, um die Liste der Abschnitte anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="7a901-117">For every retrieved notebook, call `GET ~/notebooks/{notebookId}/sections` to retrieve the list of sections.</span></span>

* <span data-ttu-id="7a901-118">Rufen Sie für jedes abgerufene Notizbuch `GET ~/notebooks/{notebookId}/sectionGroups` auf, um die Liste der Abschnittsgruppen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="7a901-118">For every retrieved notebook, call `GET ~/notebooks/{notebookId}/sectionGroups` to retrieve the list of section groups.</span></span>

* <span data-ttu-id="7a901-119">Optional können Sie die Abschnittsgruppen rekursiv durchlaufen.</span><span class="sxs-lookup"><span data-stu-id="7a901-119">Optionally recursively iterate through section groups.</span></span>

<span data-ttu-id="7a901-120">Dies ist zwar (mit ein paar zusätzlichen sequenziellen Roundtrips zum Dienst) möglich, besserer wäre es jedoch, den `$expand`-Parameter zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="7a901-120">While this will work (with a few extra sequential roundtrips to the service), a better approach is to use the `$expand` query parameter.</span></span> 

```http
GET ~/notebooks?$expand=sections,sectionGroups($expand=sections)
```

<span data-ttu-id="7a901-121">Dadurch werden dieselben Ergebnisse mit einer besseren Leistung in einer Netzwerkschleife erzielt.</span><span class="sxs-lookup"><span data-stu-id="7a901-121">This will yield the same results in one network roundtrip, with better performance.</span></span>

## <a name="when-getting-all-pages-for-a-user-do-so-for-each-section-separately"></a><span data-ttu-id="7a901-122">Wenn Sie alle Seiten eines Benutzer abrufen möchten, müssen Sie dies für jeden Abschnitt separat tun.</span><span class="sxs-lookup"><span data-stu-id="7a901-122">When getting all pages for a user, do so for each section separately</span></span>

<span data-ttu-id="7a901-123">Obgleich Microsoft Graph über einen Endpunkt verfügt, um alle Seiten abzurufen, ist dies nicht die beste Möglichkeit, um alle Seiten, auf die der Benutzer Zugriff hat, anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="7a901-123">While Microsoft Graph exposes an endpoint to retrieve all pages, this isn't the best way to get all the pages the user has access to.</span></span> <span data-ttu-id="7a901-124">Wenn der Benutzer zu viele Abschnitte besitzt, kann dies zu Timeouts oder Verschlechterung der Leistung führen.</span><span class="sxs-lookup"><span data-stu-id="7a901-124">When the user has too many sections, this can lead to timeouts or bad performance.</span></span> <span data-ttu-id="7a901-125">Es ist besser, jeden Abschnitt einzeln zu durchlaufen und die Seiten für jeden Abschnitt einzeln abzurufen.</span><span class="sxs-lookup"><span data-stu-id="7a901-125">It is better to iterate each section, getting pages for each one separately.</span></span>

<span data-ttu-id="7a901-126">Anstatt diesen Aufruf zu verwenden (diese API ist seitennummeriert, sodass Sie nicht alle Seiten auf einmal abrufenden können):</span><span class="sxs-lookup"><span data-stu-id="7a901-126">For example, instead of using this call (this API is paged, so you won't be able to fetch the pages all at once):</span></span>

```http
GET ~/pages
```

<span data-ttu-id="7a901-127">Ist es besser, den folgenden Aufruf mehrmals zu verwenden (insbesondere, wenn Sie nicht alle Abschnitte benötigen):</span><span class="sxs-lookup"><span data-stu-id="7a901-127">It is better to use the following call several times (especially if you don't need all sections):</span></span>

```http
GET ~/sections/{id}/pages
```

<span data-ttu-id="7a901-128">Wenn Sie Seitenmetadaten erhalten, überschreiben Sie die standardmäßige `lastModifiedDateTime`-Sortierung.</span><span class="sxs-lookup"><span data-stu-id="7a901-128">When getting page metadata, override the default `lastModifiedDateTime` ordering.</span></span> <span data-ttu-id="7a901-129">Seiten können schneller abgerufen werden, wenn Sie nicht nach `lastModifiedDateTime` sortiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="7a901-129">It is faster to get pages when you don't have to sort them by `lastModifiedDateTime`.</span></span> <span data-ttu-id="7a901-130">Zu diesem Zweck können Sie nach einer anderen Eigenschaft sortieren, z. B:</span><span class="sxs-lookup"><span data-stu-id="7a901-130">To do this, you can sort by any other property; for example:</span></span>

```http
GET ~/sections/{id}/pages?$select=id,title,createdDateTime&$orderby=createdDateTime
```
