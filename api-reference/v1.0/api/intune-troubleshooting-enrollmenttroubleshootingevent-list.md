---
title: enrollmentTroubleshootingEvents auflisten
description: Auflisten von Eigenschaften und Beziehungen der enrollmentTroubleshootingEvent-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ba4ed35851d5cd13e60099826e5f35f60466ee6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917356"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="8af42-103">enrollmentTroubleshootingEvents auflisten</span><span class="sxs-lookup"><span data-stu-id="8af42-103">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="8af42-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8af42-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8af42-105">Auflisten von Eigenschaften und Beziehungen der [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="8af42-105">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8af42-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8af42-106">Prerequisites</span></span>
<span data-ttu-id="8af42-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8af42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8af42-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8af42-109">Permission type</span></span>|<span data-ttu-id="8af42-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8af42-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8af42-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8af42-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8af42-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8af42-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="8af42-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8af42-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8af42-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8af42-114">Not supported.</span></span>|
|<span data-ttu-id="8af42-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8af42-115">Application</span></span>|<span data-ttu-id="8af42-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8af42-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8af42-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8af42-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="8af42-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8af42-118">Request headers</span></span>
|<span data-ttu-id="8af42-119">Header</span><span class="sxs-lookup"><span data-stu-id="8af42-119">Header</span></span>|<span data-ttu-id="8af42-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8af42-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8af42-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8af42-121">Authorization</span></span>|<span data-ttu-id="8af42-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8af42-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8af42-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8af42-123">Accept</span></span>|<span data-ttu-id="8af42-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8af42-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8af42-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8af42-125">Request body</span></span>
<span data-ttu-id="8af42-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8af42-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8af42-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="8af42-127">Response</span></span>
<span data-ttu-id="8af42-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8af42-128">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8af42-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8af42-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8af42-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8af42-130">Request</span></span>
<span data-ttu-id="8af42-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8af42-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="8af42-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="8af42-132">Response</span></span>
<span data-ttu-id="8af42-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8af42-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



