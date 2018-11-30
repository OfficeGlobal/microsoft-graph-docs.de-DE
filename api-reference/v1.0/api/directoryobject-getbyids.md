---
title: Directory-Objekte aus einer Liste von IDs abrufen
description: Wählen Sie ' Abfrageoption ist nicht verfügbar für diesen Vorgang.
ms.openlocfilehash: 4a2b765d71fe799195a4afcd404ba21718fa87c8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016199"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="8e9e6-103">Directory-Objekte aus einer Liste von IDs abrufen</span><span class="sxs-lookup"><span data-stu-id="8e9e6-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="8e9e6-p101">Gibt die in einer Liste von IDs angegebenen Directory-Objekte zurück.  HINWEIS: Die zurückgegebenen Directory-Objekte sind die vollständigen Objekte mit **allen** Eigenschaften. Die Abfrageoption `$select` ist für diesen Vorgang nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="8e9e6-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="8e9e6-107">Nachfolgend sind einige gängige Verwendungsmöglichkeiten für diese Funktion aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="8e9e6-107">Some common uses for this function are to:</span></span>

* <span data-ttu-id="8e9e6-108">Auflösen von IDs, die von Funktionen zurückgegeben werden (die Sammlungen von IDs zurückgeben), z. B. [getMemberObjects](directoryobject-getmemberobjects.md) oder [getMemberGroups](directoryobject-getmembergroups.md) in ihre zugrunde liegenden Directory-Objekte.</span><span class="sxs-lookup"><span data-stu-id="8e9e6-108">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="8e9e6-109">Auflösen von durch die Anwendung permanent in einem externen Speicher gespeicherten IDs in ihre zugrunde liegenden Verzeichnisobjekte</span><span class="sxs-lookup"><span data-stu-id="8e9e6-109">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e9e6-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8e9e6-110">Permissions</span></span>

<span data-ttu-id="8e9e6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e9e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8e9e6-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8e9e6-113">Permission type</span></span>      | <span data-ttu-id="8e9e6-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8e9e6-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e9e6-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8e9e6-115">Delegated (work or school account)</span></span> | <span data-ttu-id="8e9e6-116">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8e9e6-116">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8e9e6-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8e9e6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e9e6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e9e6-118">Not supported.</span></span>    |
|<span data-ttu-id="8e9e6-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8e9e6-119">Application</span></span> | <span data-ttu-id="8e9e6-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e9e6-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e9e6-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e9e6-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="8e9e6-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8e9e6-122">Request headers</span></span>

| <span data-ttu-id="8e9e6-123">Name</span><span class="sxs-lookup"><span data-stu-id="8e9e6-123">Name</span></span>       | <span data-ttu-id="8e9e6-124">Typ</span><span class="sxs-lookup"><span data-stu-id="8e9e6-124">Type</span></span> | <span data-ttu-id="8e9e6-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e9e6-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8e9e6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e9e6-126">Authorization</span></span>  | <span data-ttu-id="8e9e6-127">string</span><span class="sxs-lookup"><span data-stu-id="8e9e6-127">string</span></span>  | <span data-ttu-id="8e9e6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8e9e6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e9e6-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8e9e6-130">Content-Type</span></span>  | <span data-ttu-id="8e9e6-131">string</span><span class="sxs-lookup"><span data-stu-id="8e9e6-131">string</span></span> | <span data-ttu-id="8e9e6-132">application/json</span><span class="sxs-lookup"><span data-stu-id="8e9e6-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e9e6-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8e9e6-133">Request body</span></span>

<span data-ttu-id="8e9e6-134">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="8e9e6-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8e9e6-135">Parameter</span><span class="sxs-lookup"><span data-stu-id="8e9e6-135">Parameter</span></span>   | <span data-ttu-id="8e9e6-136">Typ</span><span class="sxs-lookup"><span data-stu-id="8e9e6-136">Type</span></span> |<span data-ttu-id="8e9e6-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e9e6-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e9e6-138">ids</span><span class="sxs-lookup"><span data-stu-id="8e9e6-138">ids</span></span>|<span data-ttu-id="8e9e6-139">String collection</span><span class="sxs-lookup"><span data-stu-id="8e9e6-139">String collection</span></span>| <span data-ttu-id="8e9e6-p104">Eine Sammlung von IDs, für die Objekte zurückgegeben werden sollen. Sie können bis zu 1000 IDs angeben.</span><span class="sxs-lookup"><span data-stu-id="8e9e6-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="8e9e6-142">types</span><span class="sxs-lookup"><span data-stu-id="8e9e6-142">types</span></span>|<span data-ttu-id="8e9e6-143">String collection</span><span class="sxs-lookup"><span data-stu-id="8e9e6-143">String collection</span></span>| <span data-ttu-id="8e9e6-144">Eine Auflistung von Ressourcentypen, die die Ressource zu durchsuchenden Sammlungen festlegt.</span><span class="sxs-lookup"><span data-stu-id="8e9e6-144">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="8e9e6-145">Wenn nicht angegeben, ist die Standardeinstellung [DirectoryObject](../resources/directoryobject.md), die alle im Verzeichnis definierten Ressourcentypen enthält.</span><span class="sxs-lookup"><span data-stu-id="8e9e6-145">If not specified, the default is [directoryObject](../resources/directoryobject.md), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="8e9e6-146">Alle von abgeleitetes Objekt `directoryObject` können angegeben werden, in der Auflistung. Beispiel: [Benutzer](../resources/user.md), [Gruppe](../resources/group.md), [Gerät](../resources/device.md), und So weiter.</span><span class="sxs-lookup"><span data-stu-id="8e9e6-146">Any object that derives from `directoryObject` may be specified in the collection; for example: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md), and so on.</span></span> <span data-ttu-id="8e9e6-147">Die Werte sind nicht Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="8e9e6-147">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="8e9e6-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e9e6-148">Response</span></span>

<span data-ttu-id="8e9e6-149">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8e9e6-149">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e9e6-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8e9e6-150">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8e9e6-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e9e6-151">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893874940a3-97b7-68513b600544","5d6059b6368d-45f8-91e18e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a><span data-ttu-id="8e9e6-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e9e6-152">Response</span></span>

<span data-ttu-id="8e9e6-p106">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8e9e6-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
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