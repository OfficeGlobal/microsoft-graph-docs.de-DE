---
title: enrollmentTroubleshootingEvents auflisten
description: Auflisten von Eigenschaften und Beziehungen der enrollmentTroubleshootingEvent-Objekte.
ms.openlocfilehash: 7f7b2e823757ab352a9c02433548f080f0dbdcd7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065663"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="79377-103">enrollmentTroubleshootingEvents auflisten</span><span class="sxs-lookup"><span data-stu-id="79377-103">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="79377-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="79377-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79377-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="79377-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79377-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="79377-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79377-107">Auflisten von Eigenschaften und Beziehungen der [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="79377-107">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79377-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="79377-108">Prerequisites</span></span>
<span data-ttu-id="79377-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79377-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79377-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="79377-111">Permission type</span></span>|<span data-ttu-id="79377-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="79377-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79377-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="79377-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79377-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="79377-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="79377-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="79377-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79377-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79377-116">Not supported.</span></span>|
|<span data-ttu-id="79377-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="79377-117">Application</span></span>|<span data-ttu-id="79377-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79377-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79377-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="79377-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="79377-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="79377-120">Request headers</span></span>
|<span data-ttu-id="79377-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="79377-121">Header</span></span>|<span data-ttu-id="79377-122">Wert</span><span class="sxs-lookup"><span data-stu-id="79377-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79377-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79377-123">Authorization</span></span>|<span data-ttu-id="79377-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="79377-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79377-125">Accept</span><span class="sxs-lookup"><span data-stu-id="79377-125">Accept</span></span>|<span data-ttu-id="79377-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79377-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79377-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="79377-127">Request body</span></span>
<span data-ttu-id="79377-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="79377-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79377-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="79377-129">Response</span></span>
<span data-ttu-id="79377-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="79377-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79377-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="79377-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="79377-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="79377-132">Request</span></span>
<span data-ttu-id="79377-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="79377-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="79377-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="79377-134">Response</span></span>
<span data-ttu-id="79377-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79377-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
      "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value",
      "managedDeviceIdentifier": "Managed Device Identifier value",
      "operatingSystem": "Operating System value",
      "osVersion": "Os Version value",
      "userId": "User Id value",
      "deviceId": "Device Id value",
      "enrollmentType": "userEnrollment",
      "failureCategory": "authentication",
      "failureReason": "Failure Reason value"
    }
  ]
}
```





