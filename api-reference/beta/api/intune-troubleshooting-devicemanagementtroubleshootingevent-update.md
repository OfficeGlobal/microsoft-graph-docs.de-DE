---
title: deviceManagementTroubleshootingEvent aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 496404d4a12080c9809d47f834e18e7cd5c793df
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978347"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="02491-103">deviceManagementTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="02491-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="02491-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="02491-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02491-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02491-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02491-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="02491-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02491-107">Aktualisieren der Eigenschaften eines [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="02491-107">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="02491-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="02491-108">Prerequisites</span></span>
<span data-ttu-id="02491-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02491-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02491-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="02491-111">Permission type</span></span>|<span data-ttu-id="02491-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="02491-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02491-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="02491-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02491-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02491-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="02491-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="02491-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02491-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02491-116">Not supported.</span></span>|
|<span data-ttu-id="02491-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="02491-117">Application</span></span>|<span data-ttu-id="02491-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02491-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02491-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="02491-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="02491-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="02491-120">Request headers</span></span>
|<span data-ttu-id="02491-121">Header</span><span class="sxs-lookup"><span data-stu-id="02491-121">Header</span></span>|<span data-ttu-id="02491-122">Wert</span><span class="sxs-lookup"><span data-stu-id="02491-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02491-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="02491-123">Authorization</span></span>|<span data-ttu-id="02491-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="02491-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02491-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="02491-125">Accept</span></span>|<span data-ttu-id="02491-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02491-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02491-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="02491-127">Request body</span></span>
<span data-ttu-id="02491-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) an.</span><span class="sxs-lookup"><span data-stu-id="02491-128">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="02491-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="02491-129">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="02491-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="02491-130">Property</span></span>|<span data-ttu-id="02491-131">Typ</span><span class="sxs-lookup"><span data-stu-id="02491-131">Type</span></span>|<span data-ttu-id="02491-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02491-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02491-133">id</span><span class="sxs-lookup"><span data-stu-id="02491-133">id</span></span>|<span data-ttu-id="02491-134">String</span><span class="sxs-lookup"><span data-stu-id="02491-134">String</span></span>|<span data-ttu-id="02491-135">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="02491-135">UUID for the object</span></span>|
|<span data-ttu-id="02491-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="02491-136">eventDateTime</span></span>|<span data-ttu-id="02491-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02491-137">DateTimeOffset</span></span>|<span data-ttu-id="02491-138">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="02491-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="02491-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="02491-139">correlationId</span></span>|<span data-ttu-id="02491-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="02491-140">String</span></span>|<span data-ttu-id="02491-141">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="02491-141">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="02491-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="02491-142">Response</span></span>
<span data-ttu-id="02491-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02491-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02491-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="02491-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="02491-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="02491-145">Request</span></span>
<span data-ttu-id="02491-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="02491-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 104

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="02491-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="02491-147">Response</span></span>
<span data-ttu-id="02491-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02491-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





