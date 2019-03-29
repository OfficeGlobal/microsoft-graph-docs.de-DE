---
title: deviceManagementTroubleshootingEvent abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceManagementTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58199676d28fe8d58316275b9cff6da341dad22b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980383"
---
# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="46e33-103">deviceManagementTroubleshootingEvent abrufen</span><span class="sxs-lookup"><span data-stu-id="46e33-103">Get deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="46e33-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="46e33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46e33-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="46e33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46e33-106">Lesen von Eigenschaften und Beziehungen des [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="46e33-106">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46e33-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="46e33-107">Prerequisites</span></span>
<span data-ttu-id="46e33-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46e33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46e33-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="46e33-110">Permission type</span></span>|<span data-ttu-id="46e33-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="46e33-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46e33-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="46e33-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46e33-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="46e33-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="46e33-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="46e33-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46e33-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46e33-115">Not supported.</span></span>|
|<span data-ttu-id="46e33-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="46e33-116">Application</span></span>|<span data-ttu-id="46e33-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46e33-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46e33-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="46e33-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46e33-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="46e33-119">Optional query parameters</span></span>
<span data-ttu-id="46e33-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="46e33-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46e33-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="46e33-121">Request headers</span></span>
|<span data-ttu-id="46e33-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="46e33-122">Header</span></span>|<span data-ttu-id="46e33-123">Wert</span><span class="sxs-lookup"><span data-stu-id="46e33-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46e33-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="46e33-124">Authorization</span></span>|<span data-ttu-id="46e33-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="46e33-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46e33-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="46e33-126">Accept</span></span>|<span data-ttu-id="46e33-127">application/json</span><span class="sxs-lookup"><span data-stu-id="46e33-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46e33-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="46e33-128">Request body</span></span>
<span data-ttu-id="46e33-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="46e33-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46e33-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="46e33-130">Response</span></span>
<span data-ttu-id="46e33-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46e33-131">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46e33-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="46e33-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="46e33-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="46e33-133">Request</span></span>
<span data-ttu-id="46e33-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="46e33-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="46e33-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="46e33-135">Response</span></span>
<span data-ttu-id="46e33-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46e33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 972

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
    "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
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
    ]
  }
}
```




