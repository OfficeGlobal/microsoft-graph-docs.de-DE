---
title: Leitfaden zu Einschränkungen in Microsoft Graph
description: Durch Einschränkungen wird die Anzahl der gleichzeitigen Aufrufe an einen Dienst begrenzt, um eine Überlastung von Ressourcen zu verhindern. Microsoft Graph ist für die Verarbeitung einer großen Menge von Anforderungen konzipiert. Wenn die Anzahl der Anforderungen jedoch zu hoch ist und zu einer Überlastung führen könnte, können Einschränkungen dazu beitragen, die optimale Leistung und Zuverlässigkeit des Microsoft Graph-Diensts aufrechtzuerhalten.
ms.openlocfilehash: dfe7fed3efc01932137df00d6d62ad069faf64cd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092212"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="50def-105">Leitfaden zu Einschränkungen in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="50def-105">Microsoft Graph throttling guidance</span></span>


<span data-ttu-id="50def-p102">Durch Einschränkungen wird die Anzahl der gleichzeitigen Aufrufe an einen Dienst begrenzt, um eine Überlastung von Ressourcen zu verhindern. Microsoft Graph ist für die Verarbeitung einer großen Menge von Anforderungen konzipiert. Wenn die Anzahl der Anforderungen jedoch zu hoch ist und zu einer Überlastung führen könnte, können Einschränkungen dazu beitragen, die optimale Leistung und Zuverlässigkeit des Microsoft Graph-Diensts aufrechtzuerhalten.</span><span class="sxs-lookup"><span data-stu-id="50def-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="50def-p103">Einschränkungsgrenzwerte variieren je nach Szenario. Wenn Sie beispielsweise eine große Anzahl von Schreibvorgängen ausführen, ist eine Einschränkung wahrscheinlicher, als wenn nur Lesevorgänge ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="50def-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="50def-111">Was passiert im Fall einer Einschränkung?</span><span class="sxs-lookup"><span data-stu-id="50def-111">What happens when throttling occurs?</span></span>

<span data-ttu-id="50def-p104">Wenn ein Einschränkungsschwellenwert überschritten wird, begrenzt Microsoft Graph alle weiteren Anforderungen von diesem Client für einen bestimmten Zeitraum. Im Fall einer Einschränkung gibt Microsoft Graph den HTTP-Statuscode 429 (zu viele Anforderungen) zurück, und bei den Anforderungen tritt ein Fehler auf. Eine vorgeschlagene Wartezeit wird im Antwortheader der nicht ausgeführten Anforderung zurückgegeben. Das Einschränkungsverhalten kann vom Typ und der Anzahl der Anforderungen abhängen. Wenn z. B. eine große Menge von Anforderungen vorliegt, werden alle Anforderungstypen eingeschränkt. Die Schwellenwerte variieren je nach Anforderungstyp. Daher kann der Fall eintreten, dass Schreibvorgänge eingeschränkt werden, Lesevorgänge jedoch weiterhin zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="50def-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span> 

## <a name="common-throttling-scenarios"></a><span data-ttu-id="50def-119">Allgemeine Einschränkungsszenarien</span><span class="sxs-lookup"><span data-stu-id="50def-119">Common throttling scenarios</span></span>

<span data-ttu-id="50def-120">Zu den häufigsten Ursachen für die Einschränkung von Clients zählen folgende:</span><span class="sxs-lookup"><span data-stu-id="50def-120">The most common causes of throttling of clients include:</span></span>

* <span data-ttu-id="50def-121">Eine große Anzahl von Anforderungen in allen Anwendungen in einem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="50def-121">A large number of requests across all applications in a tenant.</span></span>
* <span data-ttu-id="50def-122">Eine große Anzahl von Anforderungen von einer bestimmten Anwendung in allen Mandanten.</span><span class="sxs-lookup"><span data-stu-id="50def-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="50def-123">Bewährte Methoden zum Behandeln der Einschränkungen</span><span class="sxs-lookup"><span data-stu-id="50def-123">Best practices to handle throttling</span></span>

<span data-ttu-id="50def-124">Im Folgenden finden Sie bewährte Methoden für den Umgang mit Einschränkungen:</span><span class="sxs-lookup"><span data-stu-id="50def-124">The following are best practices for handling throttling:</span></span>

* <span data-ttu-id="50def-125">Verringern Sie die Anzahl der Vorgänge pro Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50def-125">Reduce the number of operations per request.</span></span>
* <span data-ttu-id="50def-126">Verringern Sie die Häufigkeit von Aufrufen.</span><span class="sxs-lookup"><span data-stu-id="50def-126">Reduce the frequency of calls.</span></span>
* <span data-ttu-id="50def-127">Vermeiden Sie sofortige Wiederholungsversuche, da alle Anforderungen auf Ihre Nutzungsgrenzwerte angerechnet werden.</span><span class="sxs-lookup"><span data-stu-id="50def-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="50def-p105">Wenn Sie Fehlerbehandlung implementieren, verwenden Sie den HTTP-Fehlercode 429 zur Erkennung von Einschränkungen. Im Antwortheader der Fehlerantwort ist das Feld *Retry-After* enthalten. Das Zurückhalten von Anforderungen unter Anwendung der *Retry-After*-Verzögerung ist die schnellste Methode der Wiederherstellung nach Auftreten einer Einschränkung, da Microsoft Graph den Ressourceneinsatz weiterhin protokolliert, während ein Client eingeschränkt ist.</span><span class="sxs-lookup"><span data-stu-id="50def-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the *Retry-After* field in the response header. Backing off requests using the *Retry-After* delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="50def-131">Warten Sie die im Feld *Retry-After* angegebene Anzahl von Sekunden.</span><span class="sxs-lookup"><span data-stu-id="50def-131">Wait the number of seconds specified in the *Retry-After* field.</span></span>
2. <span data-ttu-id="50def-132">Wiederholen Sie die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50def-132">Retry the request.</span></span>
3. <span data-ttu-id="50def-p106">Wenn die Anforderung erneut nicht ausgeführt und der Fehlercode 429 zurückgegeben wird, unterliegen Sie weiterhin einer Einschränkung. Wiederholen Sie die Anforderung unter Anwendung der empfohlenen Retry-After-Verzögerung so lange, bis die Anforderung erfolgreich ist.</span><span class="sxs-lookup"><span data-stu-id="50def-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended Retry-After delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="50def-135">Folgende Ressourcen bieten derzeit einen Retry-After-Header:</span><span class="sxs-lookup"><span data-stu-id="50def-135">The following resources currently provide a retry-after header:</span></span>
- [<span data-ttu-id="50def-136">Benutzer</span><span class="sxs-lookup"><span data-stu-id="50def-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="50def-137">Foto</span><span class="sxs-lookup"><span data-stu-id="50def-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="50def-138">E-Mail</span><span class="sxs-lookup"><span data-stu-id="50def-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="50def-139">Kalender (Benutzer und Gruppen)</span><span class="sxs-lookup"><span data-stu-id="50def-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="50def-140">Kontakt</span><span class="sxs-lookup"><span data-stu-id="50def-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="50def-141">Anlage</span><span class="sxs-lookup"><span data-stu-id="50def-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="50def-142">Gruppenunterhaltungen</span><span class="sxs-lookup"><span data-stu-id="50def-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="50def-143">Personen und soziale Netzwerke</span><span class="sxs-lookup"><span data-stu-id="50def-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="50def-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="50def-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)

<span data-ttu-id="50def-145">Eine ausführlichere Erläuterung zum Thema Einschränkung in der Microsoft Cloud finden Sie unter [Throttling](https://msdn.microsoft.com/library/office/dn589798.aspx).</span><span class="sxs-lookup"><span data-stu-id="50def-145">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://msdn.microsoft.com/library/office/dn589798.aspx).</span></span>
