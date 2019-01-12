---
title: deviceManagementTroubleshootingEvent erstellen
description: Erstellen eines neuen deviceManagementTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c0fd0e5ddceec3e3aa4ffae3507635286d664df8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922599"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="018dc-103">deviceManagementTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="018dc-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="018dc-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="018dc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="018dc-105">Erstellen eines neuen [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="018dc-105">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="018dc-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="018dc-106">Prerequisites</span></span>
<span data-ttu-id="018dc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="018dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="018dc-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="018dc-109">Permission type</span></span>|<span data-ttu-id="018dc-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="018dc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="018dc-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="018dc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="018dc-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="018dc-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="018dc-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="018dc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="018dc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="018dc-114">Not supported.</span></span>|
|<span data-ttu-id="018dc-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="018dc-115">Application</span></span>|<span data-ttu-id="018dc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="018dc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="018dc-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="018dc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="018dc-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="018dc-118">Request headers</span></span>
|<span data-ttu-id="018dc-119">Header</span><span class="sxs-lookup"><span data-stu-id="018dc-119">Header</span></span>|<span data-ttu-id="018dc-120">Wert</span><span class="sxs-lookup"><span data-stu-id="018dc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="018dc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="018dc-121">Authorization</span></span>|<span data-ttu-id="018dc-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="018dc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="018dc-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="018dc-123">Accept</span></span>|<span data-ttu-id="018dc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="018dc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="018dc-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="018dc-125">Request body</span></span>
<span data-ttu-id="018dc-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementTroubleshootingEvent an.</span><span class="sxs-lookup"><span data-stu-id="018dc-126">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="018dc-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="018dc-127">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="018dc-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="018dc-128">Property</span></span>|<span data-ttu-id="018dc-129">Typ</span><span class="sxs-lookup"><span data-stu-id="018dc-129">Type</span></span>|<span data-ttu-id="018dc-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="018dc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="018dc-131">id</span><span class="sxs-lookup"><span data-stu-id="018dc-131">id</span></span>|<span data-ttu-id="018dc-132">String</span><span class="sxs-lookup"><span data-stu-id="018dc-132">String</span></span>|<span data-ttu-id="018dc-133">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="018dc-133">UUID for the object</span></span>|
|<span data-ttu-id="018dc-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="018dc-134">eventDateTime</span></span>|<span data-ttu-id="018dc-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="018dc-135">DateTimeOffset</span></span>|<span data-ttu-id="018dc-136">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="018dc-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="018dc-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="018dc-137">correlationId</span></span>|<span data-ttu-id="018dc-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="018dc-138">String</span></span>|<span data-ttu-id="018dc-139">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="018dc-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="018dc-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="018dc-140">Response</span></span>
<span data-ttu-id="018dc-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="018dc-141">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="018dc-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="018dc-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="018dc-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="018dc-143">Request</span></span>
<span data-ttu-id="018dc-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="018dc-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="018dc-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="018dc-145">Response</span></span>
<span data-ttu-id="018dc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="018dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```



