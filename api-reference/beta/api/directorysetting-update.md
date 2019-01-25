---
title: Eine Einstellung für die Directory aktualisieren
description: Aktualisieren Sie die Eigenschaften eines bestimmten Verzeichnis Einstellung-Objekts.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: baaf6994f7052155173dd58b2c6b021939dc7ba7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529096"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="fd393-103">Eine Einstellung für die Directory aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fd393-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd393-104">Aktualisieren Sie die Eigenschaften eines bestimmten Verzeichnis Einstellung-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fd393-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="fd393-105">**Hinweis**: die Version /beta diese API ist nur auf Gruppen angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="fd393-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="fd393-106">So *Aktualisieren Sie GroupSettings*wurde die /v1.0 Version dieser API umbenannt.</span><span class="sxs-lookup"><span data-stu-id="fd393-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd393-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fd393-107">Permissions</span></span>
<span data-ttu-id="fd393-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd393-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd393-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd393-110">Permission type</span></span>      | <span data-ttu-id="fd393-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd393-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd393-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd393-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fd393-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fd393-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fd393-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd393-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd393-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd393-115">Not supported.</span></span>    |
|<span data-ttu-id="fd393-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd393-116">Application</span></span> | <span data-ttu-id="fd393-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd393-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd393-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd393-118">HTTP request</span></span>
<span data-ttu-id="fd393-119"><!-- { "blockType": "ignored" } -->Aktualisieren Sie eine gesamte Mandanten oder eine Gruppe bestimmte Einstellung.</span><span class="sxs-lookup"><span data-stu-id="fd393-119"><!-- { "blockType": "ignored" } --> Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="fd393-120">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd393-120">Optional request headers</span></span>
| <span data-ttu-id="fd393-121">Name</span><span class="sxs-lookup"><span data-stu-id="fd393-121">Name</span></span>       | <span data-ttu-id="fd393-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd393-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fd393-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd393-123">Authorization</span></span>  | <span data-ttu-id="fd393-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd393-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd393-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd393-126">Request body</span></span>
<span data-ttu-id="fd393-127">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="fd393-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="fd393-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fd393-128">Property</span></span>     | <span data-ttu-id="fd393-129">Typ</span><span class="sxs-lookup"><span data-stu-id="fd393-129">Type</span></span>   |<span data-ttu-id="fd393-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd393-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fd393-131">values</span><span class="sxs-lookup"><span data-stu-id="fd393-131">values</span></span> | <span data-ttu-id="fd393-132">settingValue</span><span class="sxs-lookup"><span data-stu-id="fd393-132">settingValue</span></span> | <span data-ttu-id="fd393-p104">Der aktualisierten Satz von Werten.  HINWEIS: Sie müssen den gesamten Sammlungssatz angeben. Sie können keinen einzelnen Wertesatz aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="fd393-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="fd393-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd393-136">Response</span></span>

<span data-ttu-id="fd393-137">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd393-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fd393-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd393-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd393-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd393-139">Request</span></span>
<span data-ttu-id="fd393-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd393-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="fd393-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd393-141">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update directorysetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
