---
title: Eine Einstellung für die Directory aktualisieren
description: Aktualisieren Sie die Eigenschaften eines bestimmten Verzeichnis Einstellung-Objekts.
author: lleonard-msft
ms.openlocfilehash: c4ff2401397b7a89d30f1513c504acaca5c71140
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308827"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="913b4-103">Eine Einstellung für die Directory aktualisieren</span><span class="sxs-lookup"><span data-stu-id="913b4-103">Update a directory setting</span></span>

> <span data-ttu-id="913b4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="913b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="913b4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="913b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="913b4-106">Aktualisieren Sie die Eigenschaften eines bestimmten Verzeichnis Einstellung-Objekts.</span><span class="sxs-lookup"><span data-stu-id="913b4-106">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="913b4-107">**Hinweis**: die Version /beta diese API ist nur auf Gruppen angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="913b4-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="913b4-108">So *Aktualisieren Sie GroupSettings*wurde die /v1.0 Version dieser API umbenannt.</span><span class="sxs-lookup"><span data-stu-id="913b4-108">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="913b4-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="913b4-109">Permissions</span></span>
<span data-ttu-id="913b4-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="913b4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="913b4-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="913b4-112">Permission type</span></span>      | <span data-ttu-id="913b4-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="913b4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="913b4-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="913b4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="913b4-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="913b4-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="913b4-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="913b4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="913b4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="913b4-117">Not supported.</span></span>    |
|<span data-ttu-id="913b4-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="913b4-118">Application</span></span> | <span data-ttu-id="913b4-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="913b4-119">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="913b4-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="913b4-120">HTTP request</span></span>
<span data-ttu-id="913b4-121"><!-- { "blockType": "ignored" } -->Aktualisieren Sie eine gesamte Mandanten oder eine Gruppe bestimmte Einstellung.</span><span class="sxs-lookup"><span data-stu-id="913b4-121"><!-- { "blockType": "ignored" } --> Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="913b4-122">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="913b4-122">Optional request headers</span></span>
| <span data-ttu-id="913b4-123">Name</span><span class="sxs-lookup"><span data-stu-id="913b4-123">Name</span></span>       | <span data-ttu-id="913b4-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="913b4-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="913b4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="913b4-125">Authorization</span></span>  | <span data-ttu-id="913b4-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="913b4-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="913b4-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="913b4-128">Request body</span></span>
<span data-ttu-id="913b4-129">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="913b4-129">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="913b4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="913b4-130">Property</span></span>     | <span data-ttu-id="913b4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="913b4-131">Type</span></span>   |<span data-ttu-id="913b4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="913b4-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="913b4-133">values</span><span class="sxs-lookup"><span data-stu-id="913b4-133">values</span></span> | <span data-ttu-id="913b4-134">settingValue</span><span class="sxs-lookup"><span data-stu-id="913b4-134">settingValue</span></span> | <span data-ttu-id="913b4-p105">Der aktualisierten Satz von Werten.  HINWEIS: Sie müssen den gesamten Sammlungssatz angeben. Sie können keinen einzelnen Wertesatz aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="913b4-p105">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="913b4-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="913b4-138">Response</span></span>

<span data-ttu-id="913b4-139">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="913b4-139">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="913b4-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="913b4-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="913b4-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="913b4-141">Request</span></span>
<span data-ttu-id="913b4-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="913b4-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_directorysetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/settings/{id}
Content-type: application/json
Content-length: 178

{
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="913b4-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="913b4-143">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update directorysetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->