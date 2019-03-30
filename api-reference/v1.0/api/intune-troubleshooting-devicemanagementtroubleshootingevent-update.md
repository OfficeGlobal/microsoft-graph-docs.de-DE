---
title: deviceManagementTroubleshootingEvent aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6681ef7f4cd0082d411a2f5559a5733c9fe55be2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988987"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="4563d-103">deviceManagementTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4563d-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="4563d-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4563d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4563d-105">Aktualisieren der Eigenschaften eines [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4563d-105">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4563d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4563d-106">Prerequisites</span></span>
<span data-ttu-id="4563d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4563d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4563d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4563d-109">Permission type</span></span>|<span data-ttu-id="4563d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4563d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4563d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4563d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4563d-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4563d-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4563d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4563d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4563d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4563d-114">Not supported.</span></span>|
|<span data-ttu-id="4563d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4563d-115">Application</span></span>|<span data-ttu-id="4563d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4563d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4563d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4563d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="4563d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4563d-118">Request headers</span></span>
|<span data-ttu-id="4563d-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4563d-119">Header</span></span>|<span data-ttu-id="4563d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4563d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4563d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4563d-121">Authorization</span></span>|<span data-ttu-id="4563d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4563d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4563d-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4563d-123">Accept</span></span>|<span data-ttu-id="4563d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4563d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4563d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4563d-125">Request body</span></span>
<span data-ttu-id="4563d-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) an.</span><span class="sxs-lookup"><span data-stu-id="4563d-126">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="4563d-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="4563d-127">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="4563d-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4563d-128">Property</span></span>|<span data-ttu-id="4563d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="4563d-129">Type</span></span>|<span data-ttu-id="4563d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4563d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4563d-131">id</span><span class="sxs-lookup"><span data-stu-id="4563d-131">id</span></span>|<span data-ttu-id="4563d-132">String</span><span class="sxs-lookup"><span data-stu-id="4563d-132">String</span></span>|<span data-ttu-id="4563d-133">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="4563d-133">UUID for the object</span></span>|
|<span data-ttu-id="4563d-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="4563d-134">eventDateTime</span></span>|<span data-ttu-id="4563d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4563d-135">DateTimeOffset</span></span>|<span data-ttu-id="4563d-136">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="4563d-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="4563d-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="4563d-137">correlationId</span></span>|<span data-ttu-id="4563d-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4563d-138">String</span></span>|<span data-ttu-id="4563d-139">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="4563d-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="4563d-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="4563d-140">Response</span></span>
<span data-ttu-id="4563d-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4563d-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4563d-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4563d-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="4563d-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4563d-143">Request</span></span>
<span data-ttu-id="4563d-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4563d-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="4563d-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="4563d-145">Response</span></span>
<span data-ttu-id="4563d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4563d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```



