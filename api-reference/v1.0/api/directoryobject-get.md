---
title: directoryObject abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs „directoryObject“ abrufen.
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 79cf534fc154257a952bef6494c3aa0124dfb928
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937236"
---
# <a name="get-directoryobject"></a><span data-ttu-id="f5070-103">directoryObject abrufen</span><span class="sxs-lookup"><span data-stu-id="f5070-103">Get directoryObject</span></span>

<span data-ttu-id="f5070-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs „directoryObject“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="f5070-104">Retrieve the properties and relationships of directoryObject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f5070-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f5070-105">Permissions</span></span>
<span data-ttu-id="f5070-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5070-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5070-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5070-108">Permission type</span></span>      | <span data-ttu-id="f5070-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5070-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5070-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5070-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f5070-111">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f5070-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f5070-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5070-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5070-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5070-113">Not supported.</span></span>    |
|<span data-ttu-id="f5070-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5070-114">Application</span></span> | <span data-ttu-id="f5070-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5070-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5070-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5070-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5070-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f5070-117">Optional query parameters</span></span>
<span data-ttu-id="f5070-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f5070-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f5070-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f5070-119">Request headers</span></span>
| <span data-ttu-id="f5070-120">Name</span><span class="sxs-lookup"><span data-stu-id="f5070-120">Name</span></span>       | <span data-ttu-id="f5070-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f5070-121">Type</span></span> | <span data-ttu-id="f5070-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5070-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f5070-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5070-123">Authorization</span></span>  | <span data-ttu-id="f5070-124">string</span><span class="sxs-lookup"><span data-stu-id="f5070-124">string</span></span>  | <span data-ttu-id="f5070-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f5070-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5070-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f5070-127">Request body</span></span>
<span data-ttu-id="f5070-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f5070-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5070-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5070-129">Response</span></span>

<span data-ttu-id="f5070-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5070-130">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5070-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f5070-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5070-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5070-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="f5070-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5070-133">Response</span></span>
<span data-ttu-id="f5070-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5070-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
