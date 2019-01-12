---
title: Abrufen von „enrollmentTroubleshootingEvent“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e22246c3401d0a45d0b1df70fa5a35bde2b253c3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940008"
---
# <a name="get-enrollmenttroubleshootingevent"></a><span data-ttu-id="51570-103">Abrufen von „enrollmentTroubleshootingEvent“</span><span class="sxs-lookup"><span data-stu-id="51570-103">Get enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="51570-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="51570-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51570-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="51570-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51570-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="51570-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51570-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="51570-107">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51570-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="51570-108">Prerequisites</span></span>
<span data-ttu-id="51570-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51570-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51570-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51570-111">Permission type</span></span>|<span data-ttu-id="51570-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51570-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51570-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51570-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51570-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="51570-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="51570-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51570-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51570-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51570-116">Not supported.</span></span>|
|<span data-ttu-id="51570-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51570-117">Application</span></span>|<span data-ttu-id="51570-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51570-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51570-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="51570-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51570-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="51570-120">Optional query parameters</span></span>
<span data-ttu-id="51570-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="51570-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="51570-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="51570-122">Request headers</span></span>
|<span data-ttu-id="51570-123">Header</span><span class="sxs-lookup"><span data-stu-id="51570-123">Header</span></span>|<span data-ttu-id="51570-124">Wert</span><span class="sxs-lookup"><span data-stu-id="51570-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51570-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="51570-125">Authorization</span></span>|<span data-ttu-id="51570-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="51570-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51570-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="51570-127">Accept</span></span>|<span data-ttu-id="51570-128">application/json</span><span class="sxs-lookup"><span data-stu-id="51570-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51570-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="51570-129">Request body</span></span>
<span data-ttu-id="51570-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="51570-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51570-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="51570-131">Response</span></span>
<span data-ttu-id="51570-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="51570-132">If successful, this method returns a `200 OK` response code and [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51570-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="51570-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="51570-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="51570-134">Request</span></span>
<span data-ttu-id="51570-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="51570-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="51570-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="51570-136">Response</span></span>
<span data-ttu-id="51570-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51570-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 601

{
  "value": {
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
}
```





