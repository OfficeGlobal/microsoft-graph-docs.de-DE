---
title: Gerät erstellen
description: Erstellen Sie ein neues Gerät.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4749b8cbd40a05de4d7b6c43b5cef7907d345add
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833257"
---
# <a name="create-device"></a><span data-ttu-id="bc794-103">Gerät erstellen</span><span class="sxs-lookup"><span data-stu-id="bc794-103">Create device</span></span>

> <span data-ttu-id="bc794-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bc794-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc794-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bc794-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc794-106">Erstellen Sie ein neues Gerät.</span><span class="sxs-lookup"><span data-stu-id="bc794-106">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc794-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bc794-107">Permissions</span></span>
<span data-ttu-id="bc794-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc794-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bc794-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc794-110">Permission type</span></span>      | <span data-ttu-id="bc794-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc794-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc794-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc794-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bc794-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bc794-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bc794-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc794-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc794-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc794-115">Not supported.</span></span>    |
|<span data-ttu-id="bc794-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc794-116">Application</span></span> | <span data-ttu-id="bc794-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc794-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc794-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc794-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="bc794-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc794-119">Request headers</span></span>
| <span data-ttu-id="bc794-120">Name</span><span class="sxs-lookup"><span data-stu-id="bc794-120">Name</span></span>       | <span data-ttu-id="bc794-121">Typ</span><span class="sxs-lookup"><span data-stu-id="bc794-121">Type</span></span> | <span data-ttu-id="bc794-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc794-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bc794-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc794-123">Authorization</span></span>  | <span data-ttu-id="bc794-124">string</span><span class="sxs-lookup"><span data-stu-id="bc794-124">string</span></span>  | <span data-ttu-id="bc794-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bc794-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc794-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc794-127">Request body</span></span>
<span data-ttu-id="bc794-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [device](../resources/device.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="bc794-128">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="bc794-129">Da die Ressource **Gerät** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `POST` Vorgang und Hinzufügen von benutzerdefinierten Eigenschaften mit Ihren eigenen Daten auf die Geräteinstanz beim Erstellen.</span><span class="sxs-lookup"><span data-stu-id="bc794-129">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="bc794-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc794-130">Response</span></span>

<span data-ttu-id="bc794-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [device](../resources/device.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc794-131">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc794-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc794-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc794-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc794-133">Request</span></span>
<span data-ttu-id="bc794-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bc794-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="bc794-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [device](../resources/device.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="bc794-135">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bc794-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc794-136">Response</span></span>
<span data-ttu-id="bc794-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc794-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="bc794-140">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="bc794-140">See also</span></span>

- [<span data-ttu-id="bc794-141">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="bc794-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bc794-142">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="bc794-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="bc794-143">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="bc794-143">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
