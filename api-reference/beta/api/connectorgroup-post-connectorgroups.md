---
title: Erstellen von connectorGroup
description: Verwenden Sie diese API, um eine neue ConnectorGroup erstellen.
localization_priority: Normal
ms.openlocfilehash: 233a80366c89b8cba31bd24e5d69b3a83fc20d1c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509448"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="58ea6-103">Erstellen von connectorGroup</span><span class="sxs-lookup"><span data-stu-id="58ea6-103">Create connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58ea6-104">Verwenden Sie diese API, um eine neue ConnectorGroup erstellen.</span><span class="sxs-lookup"><span data-stu-id="58ea6-104">Use this API to create a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="58ea6-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="58ea6-105">Permissions</span></span>
<span data-ttu-id="58ea6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58ea6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58ea6-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58ea6-108">Permission type</span></span>      | <span data-ttu-id="58ea6-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58ea6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58ea6-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58ea6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="58ea6-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="58ea6-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="58ea6-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58ea6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58ea6-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58ea6-113">Not supported.</span></span>    |
|<span data-ttu-id="58ea6-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58ea6-114">Application</span></span> | <span data-ttu-id="58ea6-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58ea6-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58ea6-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58ea6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups

```
## <a name="request-headers"></a><span data-ttu-id="58ea6-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58ea6-117">Request headers</span></span>
| <span data-ttu-id="58ea6-118">Name</span><span class="sxs-lookup"><span data-stu-id="58ea6-118">Name</span></span>       | <span data-ttu-id="58ea6-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58ea6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="58ea6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="58ea6-120">Authorization</span></span>  | <span data-ttu-id="58ea6-121">Bearer </span><span class="sxs-lookup"><span data-stu-id="58ea6-121">Bearer.</span></span> <span data-ttu-id="58ea6-122">Benötigte</span><span class="sxs-lookup"><span data-stu-id="58ea6-122">Requried</span></span>|

## <a name="request-body"></a><span data-ttu-id="58ea6-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58ea6-123">Request body</span></span>
<span data-ttu-id="58ea6-124">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [ConnectorGroup](../resources/connectorgroup.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="58ea6-124">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="58ea6-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="58ea6-125">Response</span></span>

<span data-ttu-id="58ea6-126">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [ConnectorGroup](../resources/connectorgroup.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="58ea6-126">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58ea6-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58ea6-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58ea6-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58ea6-128">Request</span></span>
<span data-ttu-id="58ea6-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58ea6-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connectorgroups"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false
}
```
<span data-ttu-id="58ea6-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [ConnectorGroup](../resources/connectorgroup.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="58ea6-130">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="58ea6-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="58ea6-131">Response</span></span>
<span data-ttu-id="58ea6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58ea6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-post-connectorgroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
