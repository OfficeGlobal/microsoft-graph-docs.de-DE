---
title: enrollmentTroubleshootingEvents auflisten
description: Auflisten von Eigenschaften und Beziehungen der enrollmentTroubleshootingEvent-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0fbe2d03a96af0dfe28fe08ce9bdd7e3a06f6c5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960517"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="f77aa-103">enrollmentTroubleshootingEvents auflisten</span><span class="sxs-lookup"><span data-stu-id="f77aa-103">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="f77aa-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f77aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f77aa-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f77aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f77aa-106">Auflisten von Eigenschaften und Beziehungen der [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="f77aa-106">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f77aa-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f77aa-107">Prerequisites</span></span>
<span data-ttu-id="f77aa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f77aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f77aa-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f77aa-110">Permission type</span></span>|<span data-ttu-id="f77aa-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f77aa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f77aa-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f77aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f77aa-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f77aa-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f77aa-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f77aa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f77aa-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f77aa-115">Not supported.</span></span>|
|<span data-ttu-id="f77aa-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f77aa-116">Application</span></span>|<span data-ttu-id="f77aa-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f77aa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f77aa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f77aa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="f77aa-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f77aa-119">Request headers</span></span>
|<span data-ttu-id="f77aa-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f77aa-120">Header</span></span>|<span data-ttu-id="f77aa-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f77aa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f77aa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f77aa-122">Authorization</span></span>|<span data-ttu-id="f77aa-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f77aa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f77aa-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f77aa-124">Accept</span></span>|<span data-ttu-id="f77aa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f77aa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f77aa-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f77aa-126">Request body</span></span>
<span data-ttu-id="f77aa-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f77aa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f77aa-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="f77aa-128">Response</span></span>
<span data-ttu-id="f77aa-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f77aa-129">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f77aa-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f77aa-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f77aa-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f77aa-131">Request</span></span>
<span data-ttu-id="f77aa-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f77aa-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="f77aa-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f77aa-133">Response</span></span>
<span data-ttu-id="f77aa-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f77aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1400

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
      "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value",
      "troubleshootingErrorDetails": {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
        "context": "Context value",
        "failure": "Failure value",
        "failureDetails": "Failure Details value",
        "remediation": "Remediation value",
        "resources": [
          {
            "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
            "text": "Text value",
            "link": "Link value"
          }
        ]
      },
      "eventName": "Event Name value",
      "additionalInformation": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
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




