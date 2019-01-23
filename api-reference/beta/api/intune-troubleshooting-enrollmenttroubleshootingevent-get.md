---
title: Abrufen von „enrollmentTroubleshootingEvent“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs enrollmentTroubleshootingEvent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 46016764cc47cdcae6b54f1bb8fc5a0f8b7e902f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421060"
---
# <a name="get-enrollmenttroubleshootingevent"></a><span data-ttu-id="3b289-103">Abrufen von „enrollmentTroubleshootingEvent“</span><span class="sxs-lookup"><span data-stu-id="3b289-103">Get enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="3b289-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3b289-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3b289-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b289-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b289-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3b289-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b289-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3b289-107">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b289-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3b289-108">Prerequisites</span></span>
<span data-ttu-id="3b289-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3b289-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3b289-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b289-111">Permission type</span></span>|<span data-ttu-id="3b289-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b289-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b289-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b289-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b289-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b289-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3b289-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b289-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b289-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b289-116">Not supported.</span></span>|
|<span data-ttu-id="3b289-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b289-117">Application</span></span>|<span data-ttu-id="3b289-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b289-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b289-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b289-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b289-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3b289-120">Optional query parameters</span></span>
<span data-ttu-id="3b289-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3b289-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b289-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b289-122">Request headers</span></span>
|<span data-ttu-id="3b289-123">Header</span><span class="sxs-lookup"><span data-stu-id="3b289-123">Header</span></span>|<span data-ttu-id="3b289-124">Wert</span><span class="sxs-lookup"><span data-stu-id="3b289-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b289-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3b289-125">Authorization</span></span>|<span data-ttu-id="3b289-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3b289-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b289-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3b289-127">Accept</span></span>|<span data-ttu-id="3b289-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3b289-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b289-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b289-129">Request body</span></span>
<span data-ttu-id="3b289-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3b289-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b289-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b289-131">Response</span></span>
<span data-ttu-id="3b289-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3b289-132">If successful, this method returns a `200 OK` response code and [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b289-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b289-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b289-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b289-134">Request</span></span>
<span data-ttu-id="3b289-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b289-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="3b289-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b289-136">Response</span></span>
<span data-ttu-id="3b289-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b289-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




