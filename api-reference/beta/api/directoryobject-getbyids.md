---
title: Directory-Objekte aus einer Liste von IDs abrufen
description: Wählen Sie ' Abfrageoption ist nicht verfügbar für diesen Vorgang.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 256292a1610972b8a8cbe6026344300af29b1c55
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945972"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="c88d0-103">Directory-Objekte aus einer Liste von IDs abrufen</span><span class="sxs-lookup"><span data-stu-id="c88d0-103">Get directory objects from a list of ids</span></span>

> <span data-ttu-id="c88d0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c88d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c88d0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c88d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c88d0-p102">Gibt die in einer Liste von IDs angegebenen Directory-Objekte zurück.  HINWEIS: Die zurückgegebenen Directory-Objekte sind die vollständigen Objekte mit **allen** Eigenschaften. Die Abfrageoption `$select` ist für diesen Vorgang nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c88d0-p102">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="c88d0-109">Nachfolgend sind einige gängige Verwendungsmöglichkeiten für diese Funktion aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="c88d0-109">Some common uses for this function are to:</span></span>

* <span data-ttu-id="c88d0-110">Auflösen von IDs, die von Funktionen zurückgegeben werden (die Sammlungen von IDs zurückgeben), z. B. [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) oder [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta) in ihre zugrunde liegenden Directory-Objekte.</span><span class="sxs-lookup"><span data-stu-id="c88d0-110">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) or [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta)  to their backing directory objects.</span></span>
* <span data-ttu-id="c88d0-111">Auflösen von durch die Anwendung permanent in einem externen Speicher gespeicherten IDs in ihre zugrunde liegenden Verzeichnisobjekte</span><span class="sxs-lookup"><span data-stu-id="c88d0-111">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c88d0-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c88d0-112">Permissions</span></span>

<span data-ttu-id="c88d0-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c88d0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c88d0-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c88d0-115">Permission type</span></span>      | <span data-ttu-id="c88d0-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c88d0-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c88d0-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c88d0-117">Delegated (work or school account)</span></span> | <span data-ttu-id="c88d0-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c88d0-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="c88d0-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c88d0-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c88d0-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c88d0-120">Not supported.</span></span>    |
|<span data-ttu-id="c88d0-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c88d0-121">Application</span></span> | <span data-ttu-id="c88d0-122">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c88d0-122">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c88d0-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c88d0-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="c88d0-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c88d0-124">Request headers</span></span>

| <span data-ttu-id="c88d0-125">Name</span><span class="sxs-lookup"><span data-stu-id="c88d0-125">Name</span></span>       | <span data-ttu-id="c88d0-126">Typ</span><span class="sxs-lookup"><span data-stu-id="c88d0-126">Type</span></span> | <span data-ttu-id="c88d0-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c88d0-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c88d0-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c88d0-128">Authorization</span></span>  | <span data-ttu-id="c88d0-129">string</span><span class="sxs-lookup"><span data-stu-id="c88d0-129">string</span></span>  | <span data-ttu-id="c88d0-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c88d0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c88d0-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c88d0-132">Content-Type</span></span>  | <span data-ttu-id="c88d0-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c88d0-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c88d0-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c88d0-134">Request body</span></span>

<span data-ttu-id="c88d0-135">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c88d0-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c88d0-136">Parameter</span><span class="sxs-lookup"><span data-stu-id="c88d0-136">Parameter</span></span>   | <span data-ttu-id="c88d0-137">Typ</span><span class="sxs-lookup"><span data-stu-id="c88d0-137">Type</span></span> |<span data-ttu-id="c88d0-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c88d0-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c88d0-139">ids</span><span class="sxs-lookup"><span data-stu-id="c88d0-139">ids</span></span>|<span data-ttu-id="c88d0-140">String collection</span><span class="sxs-lookup"><span data-stu-id="c88d0-140">String collection</span></span>| <span data-ttu-id="c88d0-p105">Eine Sammlung von IDs, für die Objekte zurückgegeben werden sollen. Sie können bis zu 1000 IDs angeben.</span><span class="sxs-lookup"><span data-stu-id="c88d0-p105">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="c88d0-143">types</span><span class="sxs-lookup"><span data-stu-id="c88d0-143">types</span></span>|<span data-ttu-id="c88d0-144">String collection</span><span class="sxs-lookup"><span data-stu-id="c88d0-144">String collection</span></span>| <span data-ttu-id="c88d0-145">Eine Auflistung von Ressourcentypen, die die Ressource zu durchsuchenden Sammlungen festlegt.</span><span class="sxs-lookup"><span data-stu-id="c88d0-145">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="c88d0-146">Wenn nicht angegeben, ist die Standardeinstellung [DirectoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), die alle im Verzeichnis definierten Ressourcentypen enthält.</span><span class="sxs-lookup"><span data-stu-id="c88d0-146">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="c88d0-147">Jedes Objekt, das von [DirectoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) abgeleitet wird, kann in der Auflistung angegeben werden. Beispiel: [Benutzer](/graph/api/resources/user?view=graph-rest-beta), [Gruppe](/graph/api/resources/group?view=graph-rest-beta), [Gerät](/graph/api/resources/device?view=graph-rest-beta), und So weiter.</span><span class="sxs-lookup"><span data-stu-id="c88d0-147">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta), and so on.</span></span> <span data-ttu-id="c88d0-148">Suche nach Verweise mit einem Partner [Cloud Lösungsanbieter](https://partner.microsoft.com/en-us/cloud-solution-provider) Organisation [DirectoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta)angeben.</span><span class="sxs-lookup"><span data-stu-id="c88d0-148">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span></span> <span data-ttu-id="c88d0-149">Wenn nicht angegeben, ist die Standardeinstellung [DirectoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), die alle im Verzeichnis, außer für Verweise auf einer Partnerorganisation [Cloud Lösungsanbieter](https://partner.microsoft.com/en-us/cloud-solution-provider) definierten Ressourcentypen enthält.</span><span class="sxs-lookup"><span data-stu-id="c88d0-149">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="c88d0-150">Die Werte sind nicht Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="c88d0-150">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="c88d0-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="c88d0-151">Response</span></span>

<span data-ttu-id="c88d0-152">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c88d0-152">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c88d0-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c88d0-153">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c88d0-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c88d0-154">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getByIds"
}-->

```http
POST https://graph.microsoft.com/beta/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a><span data-ttu-id="c88d0-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="c88d0-155">Response</span></span>

<span data-ttu-id="c88d0-p107">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c88d0-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
