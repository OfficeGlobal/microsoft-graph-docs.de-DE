---
title: Liste Benutzer Geräte
description: Rufen Sie eine Liste der Geräte für Benutzer, die Project-ROM-Funktionen zu unterstützen. Dazu gehören die Möglichkeit zum Starten einer Anwendung oder Nachricht oder Senden von Daten an eine Anwendung. Führen Sie nach der in mich einen Anruf GET / Geräten, übergeben Sie die ID des Geräts, einen Befehl auf Ihrem Gerät zu senden.
ms.openlocfilehash: b9e6132af0e16deae1a4175bfc811f74c18e1ae6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065276"
---
# <a name="list-user-devices"></a><span data-ttu-id="1a55a-105">Liste Benutzer Geräte</span><span class="sxs-lookup"><span data-stu-id="1a55a-105">List user devices</span></span>

> <span data-ttu-id="1a55a-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1a55a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a55a-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1a55a-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1a55a-108">Rufen Sie eine Liste der Geräte für Benutzer, die Project-ROM-Funktionen zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="1a55a-108">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="1a55a-109">Dazu gehören die Möglichkeit zum Starten einer Anwendung oder Nachricht oder Senden von Daten an eine Anwendung.</span><span class="sxs-lookup"><span data-stu-id="1a55a-109">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="1a55a-110">Führen Sie nach der in mich einen Anruf GET / Geräten, übergeben Sie die ID des Geräts auf Ihrem Gerät [Senden eines Befehls an](send-device-command.md) .</span><span class="sxs-lookup"><span data-stu-id="1a55a-110">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a55a-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1a55a-111">Permissions</span></span>

<span data-ttu-id="1a55a-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a55a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1a55a-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1a55a-114">Permission type</span></span>      | <span data-ttu-id="1a55a-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1a55a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a55a-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1a55a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="1a55a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a55a-117">Not supported.</span></span>    |
|<span data-ttu-id="1a55a-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1a55a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a55a-119">Device.Read</span><span class="sxs-lookup"><span data-stu-id="1a55a-119">Device.Read</span></span>    |
|<span data-ttu-id="1a55a-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1a55a-120">Application</span></span> | <span data-ttu-id="1a55a-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a55a-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a55a-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a55a-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="1a55a-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1a55a-123">Request headers</span></span>

| <span data-ttu-id="1a55a-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1a55a-124">Header</span></span> |<span data-ttu-id="1a55a-125">Wert</span><span class="sxs-lookup"><span data-stu-id="1a55a-125">Value</span></span>
|:----|:------|
|<span data-ttu-id="1a55a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a55a-126">Authorization</span></span>| <span data-ttu-id="1a55a-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1a55a-p105">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="1a55a-129">Accept</span><span class="sxs-lookup"><span data-stu-id="1a55a-129">Accept</span></span> | <span data-ttu-id="1a55a-130">application/json</span><span class="sxs-lookup"><span data-stu-id="1a55a-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a55a-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1a55a-131">Request body</span></span>
<span data-ttu-id="1a55a-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1a55a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a55a-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a55a-133">Response</span></span>

<span data-ttu-id="1a55a-134">Wenn erfolgreich, gibt diese Methode einen 200 Antwortcode und die Benutzereigenschaften Gerät im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1a55a-134">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="1a55a-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1a55a-135">Example</span></span>
<span data-ttu-id="1a55a-136">In diesem Beispiel wird die Liste der Geräte für einen Benutzer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a55a-136">This example will return the list of devices for a user.</span></span> <span data-ttu-id="1a55a-137">Auf einem Gerät mit command `me/devices/{id}/command`, müssen Sie die ID des Geräts zu erhalten, die zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="1a55a-137">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="1a55a-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a55a-138">Request</span></span>

<span data-ttu-id="1a55a-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1a55a-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="1a55a-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a55a-140">Response</span></span>

<span data-ttu-id="1a55a-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1a55a-141">The following is an example of the response.</span></span> <span data-ttu-id="1a55a-142">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="1a55a-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1a55a-143">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a55a-143">All of the properties will be returned from an actual call.</span></span>

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
