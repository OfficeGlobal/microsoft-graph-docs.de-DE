---
title: Gruppeneinstellungen auflisten
description: Mit dieser API können Sie eine Liste von Gruppeneinstellungsobjekten abrufen.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8cb245c786ef1fbede3e305fd73df74eb574393c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932364"
---
# <a name="list-group-settings"></a><span data-ttu-id="12ab0-103">Gruppeneinstellungen auflisten</span><span class="sxs-lookup"><span data-stu-id="12ab0-103">List group settings</span></span>

<span data-ttu-id="12ab0-104">Mit dieser API können Sie eine Liste von Gruppeneinstellungsobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="12ab0-104">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="12ab0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="12ab0-105">Permissions</span></span>

<span data-ttu-id="12ab0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12ab0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="12ab0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="12ab0-108">Permission type</span></span>      | <span data-ttu-id="12ab0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="12ab0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12ab0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="12ab0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="12ab0-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="12ab0-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="12ab0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="12ab0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12ab0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12ab0-113">Not supported.</span></span>    |
|<span data-ttu-id="12ab0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="12ab0-114">Application</span></span> | <span data-ttu-id="12ab0-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12ab0-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12ab0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="12ab0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="12ab0-117">Listet mandantenweite oder Gruppeneinstellungen auf.</span><span class="sxs-lookup"><span data-stu-id="12ab0-117">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="12ab0-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="12ab0-118">Optional query parameters</span></span>
<span data-ttu-id="12ab0-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="12ab0-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="12ab0-120">Hinweis: $filter wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12ab0-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12ab0-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="12ab0-121">Request headers</span></span>
| <span data-ttu-id="12ab0-122">Name</span><span class="sxs-lookup"><span data-stu-id="12ab0-122">Name</span></span> | <span data-ttu-id="12ab0-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12ab0-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="12ab0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="12ab0-124">Authorization</span></span>  | <span data-ttu-id="12ab0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12ab0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12ab0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="12ab0-127">Request body</span></span>
<span data-ttu-id="12ab0-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="12ab0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12ab0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="12ab0-129">Response</span></span>

<span data-ttu-id="12ab0-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [groupSetting](../resources/groupsetting.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12ab0-130">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12ab0-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="12ab0-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="12ab0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12ab0-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
##### <a name="response"></a><span data-ttu-id="12ab0-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="12ab0-133">Response</span></span>

<span data-ttu-id="12ab0-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12ab0-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
