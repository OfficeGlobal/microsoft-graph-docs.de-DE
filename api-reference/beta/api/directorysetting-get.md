---
title: Eine Einstellung für die Directory abrufen
description: Rufen Sie die Eigenschaften eines bestimmten Verzeichnis Einstellung-Objekts ab.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 132cfc64323a429431efa53bbe1d569f17095941
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864890"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="cebb5-103">Eine Einstellung für die Directory abrufen</span><span class="sxs-lookup"><span data-stu-id="cebb5-103">Get a directory setting</span></span>

> <span data-ttu-id="cebb5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cebb5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cebb5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cebb5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cebb5-106">Rufen Sie die Eigenschaften eines bestimmten Verzeichnis Einstellung-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="cebb5-106">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="cebb5-107">**Hinweis**: die Version /beta diese API ist nur auf Gruppen angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="cebb5-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="cebb5-108">Die /v1.0 Version dieser API wurde zum *Abrufen von GroupSettings*umbenannt.</span><span class="sxs-lookup"><span data-stu-id="cebb5-108">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="cebb5-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cebb5-109">Permissions</span></span>
<span data-ttu-id="cebb5-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cebb5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cebb5-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cebb5-112">Permission type</span></span>      | <span data-ttu-id="cebb5-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cebb5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cebb5-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cebb5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cebb5-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cebb5-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cebb5-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cebb5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cebb5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cebb5-117">Not supported.</span></span>    |
|<span data-ttu-id="cebb5-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cebb5-118">Application</span></span> | <span data-ttu-id="cebb5-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cebb5-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cebb5-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cebb5-120">HTTP request</span></span>
<span data-ttu-id="cebb5-121"><!-- { "blockType": "ignored" } -->Abrufen einer bestimmten Mandanten geltende oder gruppeneinstellung</span><span class="sxs-lookup"><span data-stu-id="cebb5-121"><!-- { "blockType": "ignored" } --> Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cebb5-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cebb5-122">Optional query parameters</span></span>
<span data-ttu-id="cebb5-123">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cebb5-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cebb5-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cebb5-124">Request headers</span></span>
| <span data-ttu-id="cebb5-125">Name</span><span class="sxs-lookup"><span data-stu-id="cebb5-125">Name</span></span>      |<span data-ttu-id="cebb5-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cebb5-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cebb5-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="cebb5-127">Authorization</span></span>  | <span data-ttu-id="cebb5-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cebb5-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cebb5-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cebb5-130">Request body</span></span>
<span data-ttu-id="cebb5-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cebb5-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cebb5-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="cebb5-132">Response</span></span>

<span data-ttu-id="cebb5-133">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Code und [Verzeichnisberechtigungen](../resources/directorysetting.md) Antwortobjekt im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="cebb5-133">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cebb5-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cebb5-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cebb5-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cebb5-135">Request</span></span>
<span data-ttu-id="cebb5-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cebb5-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```http
GET https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="cebb5-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="cebb5-137">Response</span></span>
<span data-ttu-id="cebb5-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cebb5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
