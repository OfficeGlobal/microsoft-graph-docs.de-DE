---
title: Abrufen von „enrollmentTroubleshootingEvent“
description: Lesen von Eigenschaften und Beziehungen des enrollmentTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cecb9d13a6b499902a04c28f836478d71c9cded0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958942"
---
# <a name="get-enrollmenttroubleshootingevent"></a><span data-ttu-id="cf448-103">Abrufen von „enrollmentTroubleshootingEvent“</span><span class="sxs-lookup"><span data-stu-id="cf448-103">Get enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="cf448-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cf448-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf448-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cf448-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf448-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="cf448-106">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf448-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cf448-107">Prerequisites</span></span>
<span data-ttu-id="cf448-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf448-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf448-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf448-110">Permission type</span></span>|<span data-ttu-id="cf448-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf448-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf448-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf448-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf448-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf448-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="cf448-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf448-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf448-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf448-115">Not supported.</span></span>|
|<span data-ttu-id="cf448-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf448-116">Application</span></span>|<span data-ttu-id="cf448-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf448-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf448-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf448-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf448-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cf448-119">Optional query parameters</span></span>
<span data-ttu-id="cf448-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cf448-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf448-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf448-121">Request headers</span></span>
|<span data-ttu-id="cf448-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cf448-122">Header</span></span>|<span data-ttu-id="cf448-123">Wert</span><span class="sxs-lookup"><span data-stu-id="cf448-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf448-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf448-124">Authorization</span></span>|<span data-ttu-id="cf448-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cf448-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf448-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cf448-126">Accept</span></span>|<span data-ttu-id="cf448-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cf448-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf448-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf448-128">Request body</span></span>
<span data-ttu-id="cf448-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cf448-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf448-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf448-130">Response</span></span>
<span data-ttu-id="cf448-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cf448-131">If successful, this method returns a `200 OK` response code and [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf448-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf448-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf448-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf448-133">Request</span></span>
<span data-ttu-id="cf448-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf448-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="cf448-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf448-135">Response</span></span>
<span data-ttu-id="cf448-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf448-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1318

{
  "value": {
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
}
```




