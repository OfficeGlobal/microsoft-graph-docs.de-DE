---
title: registeredOwner erstellen
description: Mit dieser API können Sie einen Benutzer als registrierten Besitzer eines Geräts hinzufügen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 24c5c7977e8989bd4b790df3ec0629f61a654422
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528746"
---
# <a name="create-registeredowner"></a><span data-ttu-id="d312b-103">registeredOwner erstellen</span><span class="sxs-lookup"><span data-stu-id="d312b-103">Create registeredOwner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d312b-104">Mit dieser API können Sie einen Benutzer als registrierten Besitzer eines Geräts hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="d312b-104">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="d312b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d312b-105">Permissions</span></span>
<span data-ttu-id="d312b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d312b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d312b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d312b-108">Permission type</span></span>      | <span data-ttu-id="d312b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d312b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d312b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d312b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d312b-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d312b-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d312b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d312b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d312b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d312b-113">Not supported.</span></span>    |
|<span data-ttu-id="d312b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d312b-114">Application</span></span> | <span data-ttu-id="d312b-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d312b-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d312b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d312b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="d312b-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d312b-117">Request headers</span></span>
| <span data-ttu-id="d312b-118">Name</span><span class="sxs-lookup"><span data-stu-id="d312b-118">Name</span></span>       | <span data-ttu-id="d312b-119">Typ</span><span class="sxs-lookup"><span data-stu-id="d312b-119">Type</span></span> | <span data-ttu-id="d312b-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d312b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d312b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d312b-121">Authorization</span></span>  | <span data-ttu-id="d312b-122">string</span><span class="sxs-lookup"><span data-stu-id="d312b-122">string</span></span>  | <span data-ttu-id="d312b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d312b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d312b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d312b-125">Request body</span></span>
<span data-ttu-id="d312b-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="d312b-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d312b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d312b-127">Response</span></span>

<span data-ttu-id="d312b-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d312b-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d312b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d312b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d312b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d312b-130">Request</span></span>
<span data-ttu-id="d312b-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d312b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredOwners/$ref
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="d312b-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="d312b-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d312b-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d312b-133">Response</span></span>
<span data-ttu-id="d312b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d312b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-post-registeredowners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
