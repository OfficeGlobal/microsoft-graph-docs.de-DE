---
title: registeredOwner erstellen
description: Mit dieser API können Sie einen Benutzer als registrierten Besitzer eines Geräts hinzufügen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 295c48c586a6ddf31b1ceef15b9f1137227ba3ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820524"
---
# <a name="create-registeredowner"></a><span data-ttu-id="4d774-103">registeredOwner erstellen</span><span class="sxs-lookup"><span data-stu-id="4d774-103">Create registeredOwner</span></span>

<span data-ttu-id="4d774-104">Mit dieser API können Sie einen Benutzer als registrierten Besitzer eines Geräts hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="4d774-104">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d774-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4d774-105">Permissions</span></span>
<span data-ttu-id="4d774-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d774-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4d774-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d774-108">Permission type</span></span>      | <span data-ttu-id="4d774-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d774-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d774-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d774-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4d774-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4d774-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4d774-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d774-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d774-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d774-113">Not supported.</span></span>    |
|<span data-ttu-id="4d774-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d774-114">Application</span></span> | <span data-ttu-id="4d774-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d774-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d774-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d774-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="4d774-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d774-117">Request headers</span></span>
| <span data-ttu-id="4d774-118">Name</span><span class="sxs-lookup"><span data-stu-id="4d774-118">Name</span></span>       | <span data-ttu-id="4d774-119">Typ</span><span class="sxs-lookup"><span data-stu-id="4d774-119">Type</span></span> | <span data-ttu-id="4d774-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d774-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4d774-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d774-121">Authorization</span></span>  | <span data-ttu-id="4d774-122">string</span><span class="sxs-lookup"><span data-stu-id="4d774-122">string</span></span>  | <span data-ttu-id="4d774-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4d774-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d774-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d774-125">Request body</span></span>
<span data-ttu-id="4d774-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4d774-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4d774-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d774-127">Response</span></span>

<span data-ttu-id="4d774-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d774-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d774-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d774-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d774-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d774-130">Request</span></span>
<span data-ttu-id="4d774-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d774-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="4d774-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4d774-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4d774-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d774-133">Response</span></span>
<span data-ttu-id="4d774-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d774-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
