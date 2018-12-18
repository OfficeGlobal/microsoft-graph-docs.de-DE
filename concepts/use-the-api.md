---
title: Verwenden der Microsoft Graph-API
description: Microsoft Graph ist eine RESTful-Web-API, mit der Sie auf Microsoft Cloud-Dienstressourcen zugreifen können. Nachdem Sie Ihre App registriert und Authentifizierungstoken für einen Benutzer oder einen Dienst abgerufen haben, können Sie Anforderungen an die Microsoft Graph-API tätigen.
author: jackson-woods
ms.openlocfilehash: 6f319540853e94497c6553b1bd44f7a8d3a33575
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340054"
---
# <a name="use-the-microsoft-graph-api"></a><span data-ttu-id="01603-104">Verwenden der Microsoft Graph-API</span><span class="sxs-lookup"><span data-stu-id="01603-104">Use the Microsoft Graph API</span></span>

<span data-ttu-id="01603-p102">Microsoft Graph ist eine RESTful-Web-API, mit der Sie auf Microsoft Cloud-Dienstressourcen zugreifen können. Nachdem Sie [Ihre App registriert](auth-register-app-v2.md) und [Authentifizierungstoken für einen Benutzer](auth-v2-user.md) oder einen [Dienst abgerufen haben](auth-v2-service.md), können Sie Anforderungen an die Microsoft Graph-API tätigen.</span><span class="sxs-lookup"><span data-stu-id="01603-p102">Microsoft Graph is a RESTful web API that enables you to access Microsoft Cloud service resources. After you [register your app](auth-register-app-v2.md) and [get authentication tokens for a user](auth-v2-user.md) or [service](auth-v2-service.md), you can make requests to the Microsoft Graph API.</span></span>

> <span data-ttu-id="01603-107">**Wichtig:**  Die Anwendung der Richtlinien für bedingten Zugriff für Microsoft Graph wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="01603-107">**Important:**  How conditional access policies apply to Microsoft Graph is changing.</span></span> <span data-ttu-id="01603-108">Anwendungen müssen aktualisiert werden, um Szenarien ausführen zu können, für die bedingte Richtlinien konfiguriert sind.</span><span class="sxs-lookup"><span data-stu-id="01603-108">Applications need to be updated to handle scenarios where conditional access policies are configured.</span></span> <span data-ttu-id="01603-109">Weitere Informationen und Anleitungen hierzu finden Sie unter [Developer-Leitfaden zum bedingten Zugriff in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).</span><span class="sxs-lookup"><span data-stu-id="01603-109">For more information and guidance, see [Developer Guidance for Azure Active Directory Conditional Access](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).</span></span>

<span data-ttu-id="01603-110">Erstellen Sie eine Anforderung, die der folgenden ähnlich ist, um in eine Ressource zu schreiben bzw. daraus zu lesen. Ressourcen können z. B. Benutzer oder E-Mail-Nachrichten sein.</span><span class="sxs-lookup"><span data-stu-id="01603-110">To read from or write to a resource such as a user or an email message, you construct a request that looks like the following.</span></span>

```http
https://graph.microsoft.com/{version}/{resource}?query-parameters
```

<span data-ttu-id="01603-111">Die Komponenten einer Anforderung umfassen Folgendes:</span><span class="sxs-lookup"><span data-stu-id="01603-111">The components of a request include:</span></span>

* <span data-ttu-id="01603-112">[HTTP-Methode](#http-methods) – Die HTTP-Methode, die in der Anforderung an Microsoft Graph verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="01603-112">[HTTP method](#http-methods) - The HTTP method used on the request to Microsoft Graph.</span></span>
* <span data-ttu-id="01603-113">[`{version}`](#version) – Die Version der Microsoft Graph-API, die Ihre Anwendung verwendet.</span><span class="sxs-lookup"><span data-stu-id="01603-113">[`{version}`](#version) - The version of the Microsoft Graph API your application is using.</span></span>
* <span data-ttu-id="01603-114">[`{resource}`](#resource) – Die Ressource in Microsoft Graph, auf die Sie verweisen.</span><span class="sxs-lookup"><span data-stu-id="01603-114">[`{resource}`](#resource) - The resource in Microsoft Graph that you're referencing.</span></span>
* <span data-ttu-id="01603-115">[Abfrageparameter](#query-parameters-optional) – Eine optionale Gruppe von Parametern zum Ändern der Anforderung oder der Antwort.</span><span class="sxs-lookup"><span data-stu-id="01603-115">[query-parameters](#query-parameters-optional) - An optional set of parameters to modify the request or response.</span></span>

<span data-ttu-id="01603-116">Nachdem Sie eine Anforderung vorgenommen haben, wird eine Antwort zurückgegeben, die Folgendes umfasst:</span><span class="sxs-lookup"><span data-stu-id="01603-116">After you make a request, a response is returned that includes:</span></span> 

* <span data-ttu-id="01603-p104">Statuscode – Ein HTTP-Statuscode, der eine erfolgreiche oder fehlerhafte Ausführung angibt. Informationen zu HTTP-Fehlercodes finden Sie unter [Fehler](errors.md).</span><span class="sxs-lookup"><span data-stu-id="01603-p104">Status code - An HTTP status code that indicates success or failure. For details about HTTP error codes, see [Errors](errors.md).</span></span>
* <span data-ttu-id="01603-p105">Antwortnachricht – Die angeforderten Daten oder das Ergebnis des Vorgangs. Die Antwortnachricht kann für einige Vorgänge leer sein.</span><span class="sxs-lookup"><span data-stu-id="01603-p105">Response message - The data that you requested or the result of the operation. The response message can be empty for some operations.</span></span>
* <span data-ttu-id="01603-p106">Der Link **Nächste** – Wenn Ihre Anforderung eine große Datenmenge zurückgibt, müssen Sie diese durch Auswählen von **Nächste** durchlaufen. Weitere Informationen finden Sie unter [Auslagern](paging.md).</span><span class="sxs-lookup"><span data-stu-id="01603-p106">**Next** link - If your request returns a lot of data, you need to page through it by choosing **Next**. For details, see [Paging](paging.md).</span></span>

## <a name="http-methods"></a><span data-ttu-id="01603-123">HTTP-Methoden</span><span class="sxs-lookup"><span data-stu-id="01603-123">HTTP methods</span></span>

<span data-ttu-id="01603-p107">Microsoft Graph verwendet die HTTP-Methode in Ihrer Anforderung, um zu ermitteln, welche Aktion Ihre Anforderung ausführt. Die API unterstützt die folgenden Methoden.</span><span class="sxs-lookup"><span data-stu-id="01603-p107">Microsoft Graph uses the HTTP method on your request to determine what your request is doing. The API supports the following methods.</span></span>


|<span data-ttu-id="01603-126">**Methode**</span><span class="sxs-lookup"><span data-stu-id="01603-126">**Method**</span></span> |<span data-ttu-id="01603-127">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="01603-127">**Description**</span></span>                             |
| :----- | :------------------------------------------- |
| <span data-ttu-id="01603-128">GET</span><span class="sxs-lookup"><span data-stu-id="01603-128">GET</span></span>    | <span data-ttu-id="01603-129">Dient zum Lesen von Daten aus einer Ressource.</span><span class="sxs-lookup"><span data-stu-id="01603-129">Read data from a resource.</span></span>                   |
| <span data-ttu-id="01603-130">POST</span><span class="sxs-lookup"><span data-stu-id="01603-130">POST</span></span>   | <span data-ttu-id="01603-131">Dient zum Erstellen einer neuen Ressource oder Durchführen einer Aktion.</span><span class="sxs-lookup"><span data-stu-id="01603-131">Create a new resource, or perform an action.</span></span> |
| <span data-ttu-id="01603-132">PATCH</span><span class="sxs-lookup"><span data-stu-id="01603-132">PATCH</span></span>  | <span data-ttu-id="01603-133">Dient zum Aktualisieren einer Ressource mit neuen Werten.</span><span class="sxs-lookup"><span data-stu-id="01603-133">Update a resource with new values.</span></span>           |
| <span data-ttu-id="01603-134">PUT</span><span class="sxs-lookup"><span data-stu-id="01603-134">PUT</span></span>    | <span data-ttu-id="01603-135">Dient zum Ersetzen einer Ressource durch eine neue.</span><span class="sxs-lookup"><span data-stu-id="01603-135">Replace a resource with a new one.</span></span>           |
| <span data-ttu-id="01603-136">DELETE</span><span class="sxs-lookup"><span data-stu-id="01603-136">DELETE</span></span> | <span data-ttu-id="01603-137">Dient zum Entfernen einer Ressource.</span><span class="sxs-lookup"><span data-stu-id="01603-137">Remove a resource.</span></span>                           |

* <span data-ttu-id="01603-138">Für die Methoden **GET** und **DELETE** ist kein Anforderungstext erforderlich.</span><span class="sxs-lookup"><span data-stu-id="01603-138">For the methods **GET** and **DELETE**, no request body is required.</span></span>
* <span data-ttu-id="01603-139">Die Methoden **POST**, **PATCH** und **PUT** erfordern einen Anforderungstext, in der Regel im JSON-Format, der zusätzliche Informationen enthält, z. B. die Werte für Eigenschaften der Ressource.</span><span class="sxs-lookup"><span data-stu-id="01603-139">The **POST**, **PATCH**, and **PUT** methods require a request body, usually specified in JSON format, that contains additional information, such as the values for properties of the resource.</span></span>

## <a name="version"></a><span data-ttu-id="01603-140">Version</span><span class="sxs-lookup"><span data-stu-id="01603-140">Version</span></span>

<span data-ttu-id="01603-141">Microsoft Graph unterstützt derzeit zwei Versionen: `v1.0` und `beta`.</span><span class="sxs-lookup"><span data-stu-id="01603-141">Microsoft Graph currently supports two versions: `v1.0` and `beta`.</span></span>

* <span data-ttu-id="01603-p108">`v1.0` umfasst allgemein verfügbare APIs. Verwenden Sie die Version 1.0 für alle Produktions-Apps.</span><span class="sxs-lookup"><span data-stu-id="01603-p108">`v1.0` includes generally available APIs. Use the v1.0 version for all production apps.</span></span>
* <span data-ttu-id="01603-p109">`beta` umfasst APIs, die sich derzeit in der Vorschau befinden. Da möglicherweise grundlegende Änderungen an unseren Beta-APIs eingeführt werden, wird empfohlen, dass Sie die Betaversion nur zum Testen von Apps verwenden, die sich in der Entwicklung befinden; verwenden Sie keine Beta-APIs in Ihren Produktions-Apps.</span><span class="sxs-lookup"><span data-stu-id="01603-p109">`beta` includes APIs that are currently in preview. Because we might introduce breaking changes to our beta APIs, we recommend that you use the beta version only to test apps that are in development; do not use beta APIs in your production apps.</span></span>

<span data-ttu-id="01603-p110">Wir freuen uns immer über Feedback zu unseren Beta-APIs. Auf unserer [UserVoice](https://officespdev.uservoice.com/)-Seite können Sie Feedback abgeben oder Features anfordern.</span><span class="sxs-lookup"><span data-stu-id="01603-p110">We are always looking for feedback on our beta APIs. To provide feedback or request features, see our [UserVoice](https://officespdev.uservoice.com/) page.</span></span>

<span data-ttu-id="01603-148">Weitere Informationen zu API-Versionen finden Sie unter [Versionsverwaltung und Support](versioning-and-support.md).</span><span class="sxs-lookup"><span data-stu-id="01603-148">For more information about API versions, see [Versioning and support](versioning-and-support.md).</span></span>

## <a name="resource"></a><span data-ttu-id="01603-149">Ressource</span><span class="sxs-lookup"><span data-stu-id="01603-149">Resource</span></span>

<span data-ttu-id="01603-p111">Ihre URL enthält die Ressourcen, mit denen Sie in der Anforderung interagieren, z. B. `me`, `users`, `groups`, `drives` und `sites`. Alle Ressourcen der obersten Ebene umfassen auch **Beziehungen**, die Sie verwenden können, um auf zusätzliche Ressourcen wie `me/messages` oder `me/drive` zuzugreifen. Sie können auch mithilfe von **Methoden** mit Ressourcen interagieren. Um beispielsweise eine E-Mail-Nachricht zu senden, verwenden Sie `me/sendMail`.</span><span class="sxs-lookup"><span data-stu-id="01603-p111">Your URL will include the resource or resources you are interacting with in the request, such as `me`, `users`, `groups`, `drives`, and `sites`. Each of the top-level resources also include **relationships**, which you can use to access additional resources, like `me/messages` or `me/drive`. You can also interact with resources using **methods**; for example, to send an email, use `me/sendMail`.</span></span>

<span data-ttu-id="01603-153">Weitere Informationen zum Navigieren in Ressourcenbeziehungen und Methoden finden Sie unter [Diagramm durchsuchen](traverse-the-graph.md).</span><span class="sxs-lookup"><span data-stu-id="01603-153">For more information about how to navigate resource relationships and methods, see [Traverse the graph](traverse-the-graph.md).</span></span> 

<span data-ttu-id="01603-p112">Für jede Ressource sind möglicherweise andere Berechtigungen für den Zugriff erforderlich. Häufig benötigen Sie zum Erstellen oder Aktualisieren einer Ressource eine höhere Ebene von Berechtigungen als zum Lesen. Ausführliche Informationen über die erforderlichen Berechtigungen finden Sie im Methodenreferenzthema.</span><span class="sxs-lookup"><span data-stu-id="01603-p112">Each resource might require different permissions to access it. You will often need a higher level of permissions to create or update a resource than to read it. For details about required permissions, see the method reference topic.</span></span> 

<span data-ttu-id="01603-157">Weitere Informationen zu Berechtigungen finden Sie unter [Berechtigungsreferenz](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="01603-157">For details about permissions, see [Permissions reference](permissions-reference.md).</span></span>

## <a name="query-parameters-optional"></a><span data-ttu-id="01603-158">Abfrageparameter (optional)</span><span class="sxs-lookup"><span data-stu-id="01603-158">Query parameters (optional)</span></span>

<span data-ttu-id="01603-p113">Sie können optionale Abfrageparameter verwenden, um die Antwort in Ihrer Microsoft Graph-App anzupassen. Verwenden Sie Abfrageparameter, um mehr oder weniger Eigenschaften als in der Standardantwort einzuschließen, die Antwort auf Elemente zu filtern, die einer benutzerdefinierten Abfrage entsprechen, oder zusätzliche Parameter für eine Methode anzugeben.</span><span class="sxs-lookup"><span data-stu-id="01603-p113">You can use optional query parameters to customize the response in your Microsoft Graph app. Use query parameters to include more or fewer properties than the default response, filter the response for items that match a custom query, or provide additional parameters for a method.</span></span>

<span data-ttu-id="01603-161">Durch Hinzufügen der folgenden Filterparameter werden beispielsweise die zurückgegebenen Nachrichten so eingeschränkt, dass nur diejenigen mit der `emailAddress`-Eigenschaft von `jon@contoso.com` zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="01603-161">For example, adding the following filter parameter restricts the messages returned to only those with the `emailAddress` property of `jon@contoso.com`.</span></span>

```http
https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

<span data-ttu-id="01603-162">Weitere Informationen zu Abfrageparametern finden Sie unter [Antworten anpassen](query-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="01603-162">For more information about query parameters, see [Customize responses](query-parameters.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="01603-163">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="01603-163">Next steps</span></span>

<span data-ttu-id="01603-p114">Sie sind nun bereit für Ihre ersten Schritte mit Microsoft Graph. Um mehr zu erfahren, gehen Sie zu [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer), um ein paar Anforderungen auszuprobieren. Versuchen Sie den [Schnellstart](https://developer.microsoft.com/graph/quick-start), oder beginnen Sie mit einem unserer [SDKs und Codebeispiele](https://developer.microsoft.com/graph/code-samples-and-sdks).</span><span class="sxs-lookup"><span data-stu-id="01603-p114">You're ready to get up and running with Microsoft Graph. To learn more, go to the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) to try out some requests, try the [Quick Start](https://developer.microsoft.com/graph/quick-start), or get started using one of our [SDKs and code samples](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>
