---
title: registeredUser erstellen
description: Mit dieser API können Sie einem Gerät einen registrierten Benutzer hinzufügen.
author: tfitzmac
ms.openlocfilehash: 765e82106fdfd23a6805a0bbda176635b279557d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353746"
---
# <a name="create-registereduser"></a><span data-ttu-id="f308a-103">registeredUser erstellen</span><span class="sxs-lookup"><span data-stu-id="f308a-103">Create registeredUser</span></span>

<span data-ttu-id="f308a-104">Mit dieser API können Sie einem Gerät einen registrierten Benutzer hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="f308a-104">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="f308a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f308a-105">Permissions</span></span>
<span data-ttu-id="f308a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f308a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f308a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f308a-108">Permission type</span></span>      | <span data-ttu-id="f308a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f308a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f308a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f308a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f308a-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f308a-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f308a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f308a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f308a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f308a-113">Not supported.</span></span>    |
|<span data-ttu-id="f308a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f308a-114">Application</span></span> | <span data-ttu-id="f308a-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f308a-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f308a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f308a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="f308a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f308a-117">Request headers</span></span>
| <span data-ttu-id="f308a-118">Name</span><span class="sxs-lookup"><span data-stu-id="f308a-118">Name</span></span>       | <span data-ttu-id="f308a-119">Typ</span><span class="sxs-lookup"><span data-stu-id="f308a-119">Type</span></span> | <span data-ttu-id="f308a-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f308a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f308a-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f308a-121">Authorization</span></span>  | <span data-ttu-id="f308a-122">string</span><span class="sxs-lookup"><span data-stu-id="f308a-122">string</span></span>  | <span data-ttu-id="f308a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f308a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f308a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f308a-125">Request body</span></span>
<span data-ttu-id="f308a-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f308a-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f308a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f308a-127">Response</span></span>

<span data-ttu-id="f308a-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f308a-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f308a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f308a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f308a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f308a-130">Request</span></span>
<span data-ttu-id="f308a-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f308a-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="f308a-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f308a-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f308a-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f308a-133">Response</span></span>
<span data-ttu-id="f308a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f308a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create registeredUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->