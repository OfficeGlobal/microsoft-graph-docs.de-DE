---
title: Eine Einstellung für die Directory abrufen
description: Rufen Sie die Eigenschaften eines bestimmten Verzeichnis Einstellung-Objekts ab.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0ad7b0137e741ff6c6766980f121838ae00d8200
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525290"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="ef533-103">Eine Einstellung für die Directory abrufen</span><span class="sxs-lookup"><span data-stu-id="ef533-103">Get a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef533-104">Rufen Sie die Eigenschaften eines bestimmten Verzeichnis Einstellung-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="ef533-104">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="ef533-105">**Hinweis**: die Version /beta diese API ist nur auf Gruppen angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="ef533-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="ef533-106">Die /v1.0 Version dieser API wurde zum *Abrufen von GroupSettings*umbenannt.</span><span class="sxs-lookup"><span data-stu-id="ef533-106">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef533-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ef533-107">Permissions</span></span>
<span data-ttu-id="ef533-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef533-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef533-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ef533-110">Permission type</span></span>      | <span data-ttu-id="ef533-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ef533-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef533-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ef533-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ef533-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ef533-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ef533-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ef533-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef533-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef533-115">Not supported.</span></span>    |
|<span data-ttu-id="ef533-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ef533-116">Application</span></span> | <span data-ttu-id="ef533-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef533-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef533-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef533-118">HTTP request</span></span>
<span data-ttu-id="ef533-119"><!-- { "blockType": "ignored" } -->Abrufen einer bestimmten Mandanten geltende oder gruppeneinstellung</span><span class="sxs-lookup"><span data-stu-id="ef533-119"><!-- { "blockType": "ignored" } --> Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ef533-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ef533-120">Optional query parameters</span></span>
<span data-ttu-id="ef533-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ef533-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef533-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ef533-122">Request headers</span></span>
| <span data-ttu-id="ef533-123">Name</span><span class="sxs-lookup"><span data-stu-id="ef533-123">Name</span></span>      |<span data-ttu-id="ef533-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef533-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ef533-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef533-125">Authorization</span></span>  | <span data-ttu-id="ef533-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ef533-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef533-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ef533-128">Request body</span></span>
<span data-ttu-id="ef533-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ef533-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef533-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef533-130">Response</span></span>

<span data-ttu-id="ef533-131">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Code und [Verzeichnisberechtigungen](../resources/directorysetting.md) Antwortobjekt im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ef533-131">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ef533-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ef533-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef533-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef533-133">Request</span></span>
<span data-ttu-id="ef533-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ef533-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```http
GET https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="ef533-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef533-135">Response</span></span>
<span data-ttu-id="ef533-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef533-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 198

{
  "id": "id-value",
  "displayName": "displayName-value",
  "settingTemplateId": "settingTemplateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
