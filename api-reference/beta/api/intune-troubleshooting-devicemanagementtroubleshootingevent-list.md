---
title: deviceManagementTroubleshootingEvents auflisten
description: Auflisten von Eigenschaften und Beziehungen der deviceManagementTroubleshootingEvent-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12d0e2ea8ee41cd67f4f297731b85bec0b0e18b6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960125"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="73819-103">deviceManagementTroubleshootingEvents auflisten</span><span class="sxs-lookup"><span data-stu-id="73819-103">List deviceManagementTroubleshootingEvents</span></span>

> <span data-ttu-id="73819-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="73819-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73819-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="73819-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73819-106">Auflisten von Eigenschaften und Beziehungen der [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="73819-106">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73819-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="73819-107">Prerequisites</span></span>
<span data-ttu-id="73819-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73819-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73819-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="73819-110">Permission type</span></span>|<span data-ttu-id="73819-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="73819-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73819-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="73819-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73819-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="73819-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="73819-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="73819-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73819-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73819-115">Not supported.</span></span>|
|<span data-ttu-id="73819-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="73819-116">Application</span></span>|<span data-ttu-id="73819-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73819-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73819-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="73819-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="73819-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="73819-119">Request headers</span></span>
|<span data-ttu-id="73819-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="73819-120">Header</span></span>|<span data-ttu-id="73819-121">Wert</span><span class="sxs-lookup"><span data-stu-id="73819-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73819-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73819-122">Authorization</span></span>|<span data-ttu-id="73819-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="73819-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73819-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="73819-124">Accept</span></span>|<span data-ttu-id="73819-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73819-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73819-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="73819-126">Request body</span></span>
<span data-ttu-id="73819-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="73819-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73819-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="73819-128">Response</span></span>
<span data-ttu-id="73819-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="73819-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73819-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="73819-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="73819-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="73819-131">Request</span></span>
<span data-ttu-id="73819-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="73819-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="73819-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="73819-133">Response</span></span>
<span data-ttu-id="73819-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73819-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1038

{
  "value": [
    {
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
  ]
}
```




