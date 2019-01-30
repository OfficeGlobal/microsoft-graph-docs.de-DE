---
title: Gerät erstellen
description: Erstellen Sie ein neues Gerät.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4ad0400a74deec35daa4e28f91cafde5310c65c1
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640518"
---
# <a name="create-device"></a><span data-ttu-id="29f21-103">Gerät erstellen</span><span class="sxs-lookup"><span data-stu-id="29f21-103">Create device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29f21-104">Erstellen Sie ein neues Gerät.</span><span class="sxs-lookup"><span data-stu-id="29f21-104">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="29f21-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="29f21-105">Permissions</span></span>
<span data-ttu-id="29f21-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29f21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="29f21-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="29f21-108">Permission type</span></span>      | <span data-ttu-id="29f21-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="29f21-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29f21-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="29f21-110">Delegated (work or school account)</span></span> | <span data-ttu-id="29f21-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29f21-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="29f21-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="29f21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29f21-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29f21-113">Not supported.</span></span>    |
|<span data-ttu-id="29f21-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="29f21-114">Application</span></span> | <span data-ttu-id="29f21-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29f21-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29f21-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="29f21-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="29f21-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="29f21-117">Request headers</span></span>
| <span data-ttu-id="29f21-118">Name</span><span class="sxs-lookup"><span data-stu-id="29f21-118">Name</span></span>       | <span data-ttu-id="29f21-119">Typ</span><span class="sxs-lookup"><span data-stu-id="29f21-119">Type</span></span> | <span data-ttu-id="29f21-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29f21-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="29f21-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="29f21-121">Authorization</span></span>  | <span data-ttu-id="29f21-122">string</span><span class="sxs-lookup"><span data-stu-id="29f21-122">string</span></span>  | <span data-ttu-id="29f21-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="29f21-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29f21-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="29f21-125">Request body</span></span>
<span data-ttu-id="29f21-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [device](../resources/device.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="29f21-126">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="29f21-127">Da die Ressource **Gerät** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `POST` Vorgang und Hinzufügen von benutzerdefinierten Eigenschaften mit Ihren eigenen Daten auf die Geräteinstanz beim Erstellen.</span><span class="sxs-lookup"><span data-stu-id="29f21-127">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="29f21-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="29f21-128">Response</span></span>

<span data-ttu-id="29f21-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [device](../resources/device.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29f21-129">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29f21-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29f21-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29f21-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="29f21-131">Request</span></span>
<span data-ttu-id="29f21-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="29f21-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}-->
```http
POST https://graph.microsoft.com/beta/devices
Content-type: application/json
Content-length: 364

{
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "type": 99,
      "identityProvider": "identityProvider-value",
      "key": "key-value"
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```
<span data-ttu-id="29f21-133">Geben Sie im Anforderungstext eine JSON-Darstellung des [device](../resources/device.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="29f21-133">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="29f21-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="29f21-134">Response</span></span>
<span data-ttu-id="29f21-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29f21-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 364

{
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "type": 99,
      "identityProvider": "identityProvider-value",
      "key": "key-value"
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```

## <a name="see-also"></a><span data-ttu-id="29f21-138">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="29f21-138">See also</span></span>

- [<span data-ttu-id="29f21-139">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="29f21-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="29f21-140">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="29f21-140">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="29f21-141">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="29f21-141">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-post-devices.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
