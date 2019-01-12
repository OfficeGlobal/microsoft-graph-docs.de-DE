---
title: deviceManagementTroubleshootingEvents auflisten
description: Auflisten von Eigenschaften und Beziehungen der deviceManagementTroubleshootingEvent-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b6ab19d049268b0880789b73e9900e3e8ad784a0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986838"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="18e64-103">deviceManagementTroubleshootingEvents auflisten</span><span class="sxs-lookup"><span data-stu-id="18e64-103">List deviceManagementTroubleshootingEvents</span></span>

> <span data-ttu-id="18e64-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="18e64-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18e64-105">Auflisten von Eigenschaften und Beziehungen der [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="18e64-105">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18e64-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="18e64-106">Prerequisites</span></span>
<span data-ttu-id="18e64-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18e64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18e64-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18e64-109">Permission type</span></span>|<span data-ttu-id="18e64-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18e64-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18e64-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18e64-111">Delegated (work or school account)</span></span>|<span data-ttu-id="18e64-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="18e64-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="18e64-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18e64-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18e64-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18e64-114">Not supported.</span></span>|
|<span data-ttu-id="18e64-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18e64-115">Application</span></span>|<span data-ttu-id="18e64-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18e64-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18e64-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18e64-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="18e64-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18e64-118">Request headers</span></span>
|<span data-ttu-id="18e64-119">Header</span><span class="sxs-lookup"><span data-stu-id="18e64-119">Header</span></span>|<span data-ttu-id="18e64-120">Wert</span><span class="sxs-lookup"><span data-stu-id="18e64-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18e64-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="18e64-121">Authorization</span></span>|<span data-ttu-id="18e64-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="18e64-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18e64-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="18e64-123">Accept</span></span>|<span data-ttu-id="18e64-124">application/json</span><span class="sxs-lookup"><span data-stu-id="18e64-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18e64-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18e64-125">Request body</span></span>
<span data-ttu-id="18e64-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="18e64-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18e64-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="18e64-127">Response</span></span>
<span data-ttu-id="18e64-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="18e64-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18e64-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18e64-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="18e64-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18e64-130">Request</span></span>
<span data-ttu-id="18e64-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18e64-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="18e64-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="18e64-132">Response</span></span>
<span data-ttu-id="18e64-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18e64-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
      "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value"
    }
  ]
}
```



