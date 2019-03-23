---
title: Aktualisieren einer Verzeichnis Einstellung
description: Aktualisieren der Eigenschaften eines bestimmten Verzeichnis Einstellungs Objekts.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1337527b7be6c8cc7f2b52f37a1698d61fa9b842
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789613"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="71070-103">Aktualisieren einer Verzeichnis Einstellung</span><span class="sxs-lookup"><span data-stu-id="71070-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71070-104">Aktualisieren der Eigenschaften eines bestimmten Verzeichnis Einstellungs Objekts.</span><span class="sxs-lookup"><span data-stu-id="71070-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="71070-105">**Hinweis**: die/Beta-Version dieser API gilt nur für Gruppen.</span><span class="sxs-lookup"><span data-stu-id="71070-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="71070-106">Die/v1.0-Version dieser API wurde in *Update groupSettings*umbenannt.</span><span class="sxs-lookup"><span data-stu-id="71070-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="71070-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="71070-107">Permissions</span></span>
<span data-ttu-id="71070-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71070-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71070-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71070-110">Permission type</span></span>      | <span data-ttu-id="71070-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71070-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71070-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71070-112">Delegated (work or school account)</span></span> | <span data-ttu-id="71070-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="71070-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="71070-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71070-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71070-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71070-115">Not supported.</span></span>    |
|<span data-ttu-id="71070-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71070-116">Application</span></span> | <span data-ttu-id="71070-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71070-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71070-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71070-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="71070-119">Aktualisiert eine mandantenweite oder gruppenspezifische Einstellung.</span><span class="sxs-lookup"><span data-stu-id="71070-119">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="71070-120">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71070-120">Optional request headers</span></span>
| <span data-ttu-id="71070-121">Name</span><span class="sxs-lookup"><span data-stu-id="71070-121">Name</span></span>       | <span data-ttu-id="71070-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71070-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="71070-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71070-123">Authorization</span></span>  | <span data-ttu-id="71070-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="71070-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71070-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71070-126">Request body</span></span>
<span data-ttu-id="71070-127">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="71070-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="71070-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71070-128">Property</span></span>     | <span data-ttu-id="71070-129">Typ</span><span class="sxs-lookup"><span data-stu-id="71070-129">Type</span></span>   |<span data-ttu-id="71070-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71070-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="71070-131">values</span><span class="sxs-lookup"><span data-stu-id="71070-131">values</span></span> | <span data-ttu-id="71070-132">[](../resources/settingvalue.md) SettingValue-Auflistung</span><span class="sxs-lookup"><span data-stu-id="71070-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="71070-133">Der aktualisierte Satz von Werten.</span><span class="sxs-lookup"><span data-stu-id="71070-133">The updated set of values.</span></span>  <span data-ttu-id="71070-134">Hinweis: Sie müssen den gesamten Sammlungssatz angeben.</span><span class="sxs-lookup"><span data-stu-id="71070-134">NOTE: You must supply the entire collection set.</span></span> <span data-ttu-id="71070-135">Sie können nicht einen einzelnen Satz von Werten aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="71070-135">You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="71070-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="71070-136">Response</span></span>

<span data-ttu-id="71070-137">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71070-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="71070-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71070-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71070-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71070-139">Request</span></span>
<span data-ttu-id="71070-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71070-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="71070-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="71070-141">Response</span></span>
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
