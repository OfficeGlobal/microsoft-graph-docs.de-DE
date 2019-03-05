---
title: enrollmentTroubleshootingEvents auflisten
description: Auflisten von Eigenschaften und Beziehungen der enrollmentTroubleshootingEvent-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4c5ed76dd35fe3077b8543be0518094698ab031
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258191"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="e73ad-103">enrollmentTroubleshootingEvents auflisten</span><span class="sxs-lookup"><span data-stu-id="e73ad-103">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="e73ad-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e73ad-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e73ad-105">Auflisten von Eigenschaften und Beziehungen der [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="e73ad-105">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e73ad-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e73ad-106">Prerequisites</span></span>
<span data-ttu-id="e73ad-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e73ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e73ad-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e73ad-109">Permission type</span></span>|<span data-ttu-id="e73ad-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e73ad-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e73ad-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e73ad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e73ad-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e73ad-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e73ad-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e73ad-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e73ad-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e73ad-114">Not supported.</span></span>|
|<span data-ttu-id="e73ad-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e73ad-115">Application</span></span>|<span data-ttu-id="e73ad-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e73ad-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e73ad-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e73ad-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="e73ad-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e73ad-118">Request headers</span></span>
|<span data-ttu-id="e73ad-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e73ad-119">Header</span></span>|<span data-ttu-id="e73ad-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e73ad-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e73ad-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e73ad-121">Authorization</span></span>|<span data-ttu-id="e73ad-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e73ad-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e73ad-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e73ad-123">Accept</span></span>|<span data-ttu-id="e73ad-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e73ad-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e73ad-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e73ad-125">Request body</span></span>
<span data-ttu-id="e73ad-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e73ad-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e73ad-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e73ad-127">Response</span></span>
<span data-ttu-id="e73ad-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e73ad-128">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e73ad-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e73ad-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e73ad-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e73ad-130">Request</span></span>
<span data-ttu-id="e73ad-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e73ad-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="e73ad-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="e73ad-132">Response</span></span>
<span data-ttu-id="e73ad-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e73ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



