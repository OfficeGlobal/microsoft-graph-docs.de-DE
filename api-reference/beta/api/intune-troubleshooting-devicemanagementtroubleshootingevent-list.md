---
title: deviceManagementTroubleshootingEvents auflisten
description: Auflisten von Eigenschaften und Beziehungen der deviceManagementTroubleshootingEvent-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 779ab783d58bd5ffb71281bd37a3fc7d0e7b9748
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393032"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="3ace0-103">deviceManagementTroubleshootingEvents auflisten</span><span class="sxs-lookup"><span data-stu-id="3ace0-103">List deviceManagementTroubleshootingEvents</span></span>

> <span data-ttu-id="3ace0-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3ace0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3ace0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3ace0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ace0-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3ace0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ace0-107">Auflisten von Eigenschaften und Beziehungen der [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="3ace0-107">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ace0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3ace0-108">Prerequisites</span></span>
<span data-ttu-id="3ace0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3ace0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3ace0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3ace0-111">Permission type</span></span>|<span data-ttu-id="3ace0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3ace0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ace0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3ace0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ace0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ace0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3ace0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3ace0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ace0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ace0-116">Not supported.</span></span>|
|<span data-ttu-id="3ace0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3ace0-117">Application</span></span>|<span data-ttu-id="3ace0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ace0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ace0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ace0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="3ace0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3ace0-120">Request headers</span></span>
|<span data-ttu-id="3ace0-121">Header</span><span class="sxs-lookup"><span data-stu-id="3ace0-121">Header</span></span>|<span data-ttu-id="3ace0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3ace0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ace0-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3ace0-123">Authorization</span></span>|<span data-ttu-id="3ace0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3ace0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ace0-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3ace0-125">Accept</span></span>|<span data-ttu-id="3ace0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ace0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ace0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3ace0-127">Request body</span></span>
<span data-ttu-id="3ace0-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3ace0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ace0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ace0-129">Response</span></span>
<span data-ttu-id="3ace0-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3ace0-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ace0-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3ace0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ace0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ace0-132">Request</span></span>
<span data-ttu-id="3ace0-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3ace0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="3ace0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ace0-134">Response</span></span>
<span data-ttu-id="3ace0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ace0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




