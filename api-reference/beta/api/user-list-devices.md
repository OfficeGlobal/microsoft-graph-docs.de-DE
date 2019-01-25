---
title: Liste Benutzer Geräte
description: Rufen Sie eine Liste der Geräte für Benutzer, die Project-ROM-Funktionen zu unterstützen. Dazu gehören die Möglichkeit zum Starten einer Anwendung oder Nachricht oder Senden von Daten an eine Anwendung. Führen Sie nach der in mich einen Anruf GET / Geräten, übergeben Sie die ID des Geräts, einen Befehl auf Ihrem Gerät zu senden.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 891f66691149106d4ff5a2951170524203eb2ea7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509525"
---
# <a name="list-user-devices"></a><span data-ttu-id="7fcae-105">Liste Benutzer Geräte</span><span class="sxs-lookup"><span data-stu-id="7fcae-105">List user devices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fcae-106">Rufen Sie eine Liste der Geräte für Benutzer, die Project-ROM-Funktionen zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="7fcae-106">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="7fcae-107">Dazu gehören die Möglichkeit zum Starten einer Anwendung oder Nachricht oder Senden von Daten an eine Anwendung.</span><span class="sxs-lookup"><span data-stu-id="7fcae-107">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="7fcae-108">Führen Sie nach der in mich einen Anruf GET / Geräten, übergeben Sie die ID des Geräts auf Ihrem Gerät [Senden eines Befehls an](send-device-command.md) .</span><span class="sxs-lookup"><span data-stu-id="7fcae-108">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fcae-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7fcae-109">Permissions</span></span>

<span data-ttu-id="7fcae-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fcae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7fcae-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7fcae-112">Permission type</span></span>      | <span data-ttu-id="7fcae-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7fcae-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fcae-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7fcae-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7fcae-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7fcae-115">Not supported.</span></span>    |
|<span data-ttu-id="7fcae-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7fcae-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fcae-117">Device.Read</span><span class="sxs-lookup"><span data-stu-id="7fcae-117">Device.Read</span></span>    |
|<span data-ttu-id="7fcae-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7fcae-118">Application</span></span> | <span data-ttu-id="7fcae-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7fcae-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fcae-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7fcae-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="7fcae-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7fcae-121">Request headers</span></span>

| <span data-ttu-id="7fcae-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7fcae-122">Header</span></span> |<span data-ttu-id="7fcae-123">Wert</span><span class="sxs-lookup"><span data-stu-id="7fcae-123">Value</span></span>
|:----|:------|
|<span data-ttu-id="7fcae-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fcae-124">Authorization</span></span>| <span data-ttu-id="7fcae-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7fcae-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="7fcae-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7fcae-127">Accept</span></span> | <span data-ttu-id="7fcae-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7fcae-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fcae-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7fcae-129">Request body</span></span>
<span data-ttu-id="7fcae-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7fcae-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fcae-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="7fcae-131">Response</span></span>

<span data-ttu-id="7fcae-132">Wenn erfolgreich, gibt diese Methode einen 200 Antwortcode und die Benutzereigenschaften Gerät im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7fcae-132">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```

<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#devices",
  "value": [
    {
      "name": "name",
      "id": "id",
      "status": "status",
      "platform": "platform",
      "kind": "formFactor",
      "model": "model",
      "manufacturer": "manufacturer",
    }
  ]
}
```

## <a name="example"></a><span data-ttu-id="7fcae-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7fcae-133">Example</span></span>
<span data-ttu-id="7fcae-134">In diesem Beispiel wird die Liste der Geräte für einen Benutzer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7fcae-134">This example will return the list of devices for a user.</span></span> <span data-ttu-id="7fcae-135">Auf einem Gerät mit command `me/devices/{id}/command`, müssen Sie die ID des Geräts zu erhalten, die zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="7fcae-135">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="7fcae-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7fcae-136">Request</span></span>

<span data-ttu-id="7fcae-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7fcae-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="7fcae-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="7fcae-138">Response</span></span>

<span data-ttu-id="7fcae-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7fcae-139">The following is an example of the response.</span></span> <span data-ttu-id="7fcae-140">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="7fcae-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7fcae-141">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7fcae-141">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 140

{
  "value": [
    {
      "Name": "JimSurface",
      "id": "6841b3db-2b55-467b-ad84-79a41a4ef665",
      "Manufacturer": "Microsoft Corporation",
      "Model": "Surface Book",
      "Kind": "Tablet",
      "Status": "Unknown",
      "Platform": "Windows"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-devices.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
