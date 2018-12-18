---
title: deviceManagementTroubleshootingEvent aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementTroubleshootingEvent-Objekts.
author: tfitzmac
ms.openlocfilehash: ec4cf8d98d51ec369739158c3cf8f6daf2e2ac8e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358807"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="0f09b-103">deviceManagementTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0f09b-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="0f09b-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0f09b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f09b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f09b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f09b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0f09b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f09b-107">Aktualisieren der Eigenschaften eines [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0f09b-107">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0f09b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0f09b-108">Prerequisites</span></span>
<span data-ttu-id="0f09b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f09b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f09b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f09b-111">Permission type</span></span>|<span data-ttu-id="0f09b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0f09b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f09b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f09b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f09b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f09b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0f09b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f09b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f09b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f09b-116">Not supported.</span></span>|
|<span data-ttu-id="0f09b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f09b-117">Application</span></span>|<span data-ttu-id="0f09b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f09b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f09b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f09b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="0f09b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f09b-120">Request headers</span></span>
|<span data-ttu-id="0f09b-121">Header</span><span class="sxs-lookup"><span data-stu-id="0f09b-121">Header</span></span>|<span data-ttu-id="0f09b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0f09b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f09b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0f09b-123">Authorization</span></span>|<span data-ttu-id="0f09b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0f09b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f09b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0f09b-125">Accept</span></span>|<span data-ttu-id="0f09b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f09b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f09b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0f09b-127">Request body</span></span>
<span data-ttu-id="0f09b-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) an.</span><span class="sxs-lookup"><span data-stu-id="0f09b-128">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="0f09b-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="0f09b-129">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="0f09b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f09b-130">Property</span></span>|<span data-ttu-id="0f09b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0f09b-131">Type</span></span>|<span data-ttu-id="0f09b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f09b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f09b-133">id</span><span class="sxs-lookup"><span data-stu-id="0f09b-133">id</span></span>|<span data-ttu-id="0f09b-134">String</span><span class="sxs-lookup"><span data-stu-id="0f09b-134">String</span></span>|<span data-ttu-id="0f09b-135">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="0f09b-135">UUID for the object</span></span>|
|<span data-ttu-id="0f09b-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="0f09b-136">eventDateTime</span></span>|<span data-ttu-id="0f09b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f09b-137">DateTimeOffset</span></span>|<span data-ttu-id="0f09b-138">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="0f09b-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="0f09b-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="0f09b-139">correlationId</span></span>|<span data-ttu-id="0f09b-140">String</span><span class="sxs-lookup"><span data-stu-id="0f09b-140">String</span></span>|<span data-ttu-id="0f09b-141">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="0f09b-141">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="0f09b-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f09b-142">Response</span></span>
<span data-ttu-id="0f09b-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f09b-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f09b-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f09b-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f09b-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f09b-145">Request</span></span>
<span data-ttu-id="0f09b-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0f09b-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 104

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="0f09b-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f09b-147">Response</span></span>
<span data-ttu-id="0f09b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f09b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





