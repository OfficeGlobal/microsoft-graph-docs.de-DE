---
title: Gerät erstellen
description: Erstellen Sie ein neues Gerät.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0d24829a057326d35b2b35e0ba72d736e3afb15c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971599"
---
# <a name="create-device"></a><span data-ttu-id="38f83-103">Gerät erstellen</span><span class="sxs-lookup"><span data-stu-id="38f83-103">Create device</span></span>

> <span data-ttu-id="38f83-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="38f83-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38f83-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="38f83-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="38f83-106">Erstellen Sie ein neues Gerät.</span><span class="sxs-lookup"><span data-stu-id="38f83-106">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="38f83-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="38f83-107">Permissions</span></span>
<span data-ttu-id="38f83-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38f83-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="38f83-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38f83-110">Permission type</span></span>      | <span data-ttu-id="38f83-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38f83-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38f83-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38f83-112">Delegated (work or school account)</span></span> | <span data-ttu-id="38f83-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="38f83-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="38f83-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38f83-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38f83-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38f83-115">Not supported.</span></span>    |
|<span data-ttu-id="38f83-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38f83-116">Application</span></span> | <span data-ttu-id="38f83-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38f83-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38f83-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38f83-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="38f83-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38f83-119">Request headers</span></span>
| <span data-ttu-id="38f83-120">Name</span><span class="sxs-lookup"><span data-stu-id="38f83-120">Name</span></span>       | <span data-ttu-id="38f83-121">Typ</span><span class="sxs-lookup"><span data-stu-id="38f83-121">Type</span></span> | <span data-ttu-id="38f83-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38f83-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="38f83-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="38f83-123">Authorization</span></span>  | <span data-ttu-id="38f83-124">string</span><span class="sxs-lookup"><span data-stu-id="38f83-124">string</span></span>  | <span data-ttu-id="38f83-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38f83-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38f83-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38f83-127">Request body</span></span>
<span data-ttu-id="38f83-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [device](../resources/device.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="38f83-128">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="38f83-129">Da die Ressource **Gerät** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `POST` Vorgang und Hinzufügen von benutzerdefinierten Eigenschaften mit Ihren eigenen Daten auf die Geräteinstanz beim Erstellen.</span><span class="sxs-lookup"><span data-stu-id="38f83-129">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="38f83-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="38f83-130">Response</span></span>

<span data-ttu-id="38f83-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [device](../resources/device.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38f83-131">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38f83-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38f83-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38f83-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38f83-133">Request</span></span>
<span data-ttu-id="38f83-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="38f83-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="38f83-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [device](../resources/device.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="38f83-135">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="38f83-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="38f83-136">Response</span></span>
<span data-ttu-id="38f83-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38f83-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="38f83-140">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="38f83-140">See also</span></span>

- [<span data-ttu-id="38f83-141">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="38f83-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="38f83-142">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="38f83-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="38f83-143">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="38f83-143">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
