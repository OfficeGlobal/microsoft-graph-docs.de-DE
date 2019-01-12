---
title: Abrufen einer Gruppeneinstellung
description: Mit dieser API können Sie die Eigenschaften eines bestimmten Gruppeneinstellungsobjekts abrufen.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d47441a66ab0b2ed3602a69f4a92a06050708f67
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936501"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="141f4-103">Abrufen einer Gruppeneinstellung</span><span class="sxs-lookup"><span data-stu-id="141f4-103">Get a group setting</span></span>

<span data-ttu-id="141f4-104">Mit dieser API können Sie die Eigenschaften eines bestimmten Gruppeneinstellungsobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="141f4-104">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="141f4-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="141f4-105">Permissions</span></span>

<span data-ttu-id="141f4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="141f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="141f4-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="141f4-108">Permission type</span></span>      | <span data-ttu-id="141f4-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="141f4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="141f4-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="141f4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="141f4-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="141f4-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="141f4-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="141f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="141f4-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="141f4-113">Not supported.</span></span>    |
|<span data-ttu-id="141f4-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="141f4-114">Application</span></span> | <span data-ttu-id="141f4-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="141f4-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="141f4-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="141f4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="141f4-117">Rufen Sie eine bestimmte Mandanten-übergreifende oder Gruppeneinstellung ab.</span><span class="sxs-lookup"><span data-stu-id="141f4-117">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="141f4-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="141f4-118">Optional query parameters</span></span>
<span data-ttu-id="141f4-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="141f4-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="141f4-120">Hinweis: $filter wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="141f4-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="141f4-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="141f4-121">Request headers</span></span>
| <span data-ttu-id="141f4-122">Name</span><span class="sxs-lookup"><span data-stu-id="141f4-122">Name</span></span> | <span data-ttu-id="141f4-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="141f4-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="141f4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="141f4-124">Authorization</span></span> | <span data-ttu-id="141f4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="141f4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="141f4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="141f4-127">Request body</span></span>

<span data-ttu-id="141f4-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="141f4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="141f4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="141f4-129">Response</span></span>

<span data-ttu-id="141f4-130">Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `200 OK` und das [groupSetting](../resources/groupsetting.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="141f4-130">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="141f4-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="141f4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="141f4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="141f4-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="141f4-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="141f4-133">Response</span></span>

<span data-ttu-id="141f4-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="141f4-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
