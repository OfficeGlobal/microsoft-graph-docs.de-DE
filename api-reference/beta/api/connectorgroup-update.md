---
title: ConnectorGroups aktualisieren
description: Aktualisieren Sie die Eigenschaften des Connectorgroup-Objekts.
localization_priority: Normal
ms.openlocfilehash: 9d6feec19552aeeebe51ba0fab07e805c6f4a2bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530111"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="a81d4-103">ConnectorGroups aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a81d4-103">Update connectorGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a81d4-104">Aktualisieren Sie die Eigenschaften des Connectorgroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a81d4-104">Update the properties of connectorgroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a81d4-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a81d4-105">Permissions</span></span>
<span data-ttu-id="a81d4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a81d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a81d4-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a81d4-108">Permission type</span></span>      | <span data-ttu-id="a81d4-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a81d4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a81d4-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a81d4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a81d4-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a81d4-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a81d4-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a81d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a81d4-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a81d4-113">Not supported.</span></span>    |
|<span data-ttu-id="a81d4-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a81d4-114">Application</span></span> | <span data-ttu-id="a81d4-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a81d4-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a81d4-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a81d4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="a81d4-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a81d4-117">Optional request headers</span></span>
| <span data-ttu-id="a81d4-118">Name</span><span class="sxs-lookup"><span data-stu-id="a81d4-118">Name</span></span>       | <span data-ttu-id="a81d4-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a81d4-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a81d4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a81d4-120">Authorization</span></span>  | <span data-ttu-id="a81d4-121">Bearer </span><span class="sxs-lookup"><span data-stu-id="a81d4-121">Bearer.</span></span> <span data-ttu-id="a81d4-122">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="a81d4-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="a81d4-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a81d4-123">Request body</span></span>
<span data-ttu-id="a81d4-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="a81d4-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a81d4-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a81d4-127">Property</span></span>     | <span data-ttu-id="a81d4-128">Typ</span><span class="sxs-lookup"><span data-stu-id="a81d4-128">Type</span></span>   |<span data-ttu-id="a81d4-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a81d4-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a81d4-130">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="a81d4-130">connectorGroupType</span></span>|<span data-ttu-id="a81d4-131">string</span><span class="sxs-lookup"><span data-stu-id="a81d4-131">string</span></span>| <span data-ttu-id="a81d4-132">Mögliche Werte sind: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="a81d4-132">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="a81d4-133">name</span><span class="sxs-lookup"><span data-stu-id="a81d4-133">name</span></span>|<span data-ttu-id="a81d4-134">String</span><span class="sxs-lookup"><span data-stu-id="a81d4-134">String</span></span>|<span data-ttu-id="a81d4-135">Der Name der ConnectorGroup.</span><span class="sxs-lookup"><span data-stu-id="a81d4-135">The name of the connectorGroup.</span></span>|

## <a name="response"></a><span data-ttu-id="a81d4-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a81d4-136">Response</span></span>

<span data-ttu-id="a81d4-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [ConnectorGroup](../resources/connectorgroup.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a81d4-137">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a81d4-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a81d4-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a81d4-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a81d4-139">Request</span></span>
<span data-ttu-id="a81d4-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a81d4-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
PATCH https://graph.microsoft.com/{ver}/connectorGroups/{id}
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
}
```
##### <a name="response"></a><span data-ttu-id="a81d4-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="a81d4-141">Response</span></span>
<span data-ttu-id="a81d4-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a81d4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
