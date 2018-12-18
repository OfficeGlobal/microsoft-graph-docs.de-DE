---
title: deviceManagementTroubleshootingEvent erstellen
description: Erstellen eines neuen deviceManagementTroubleshootingEvent-Objekts.
author: tfitzmac
ms.openlocfilehash: cef96acd7db28fd9b686c01e748532e775cf5f01
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356406"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="676fe-103">deviceManagementTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="676fe-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="676fe-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="676fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="676fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="676fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="676fe-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="676fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="676fe-107">Erstellen eines neuen [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="676fe-107">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="676fe-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="676fe-108">Prerequisites</span></span>
<span data-ttu-id="676fe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="676fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="676fe-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="676fe-111">Permission type</span></span>|<span data-ttu-id="676fe-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="676fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="676fe-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="676fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="676fe-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="676fe-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="676fe-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="676fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="676fe-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="676fe-116">Not supported.</span></span>|
|<span data-ttu-id="676fe-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="676fe-117">Application</span></span>|<span data-ttu-id="676fe-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="676fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="676fe-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="676fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="676fe-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="676fe-120">Request headers</span></span>
|<span data-ttu-id="676fe-121">Header</span><span class="sxs-lookup"><span data-stu-id="676fe-121">Header</span></span>|<span data-ttu-id="676fe-122">Wert</span><span class="sxs-lookup"><span data-stu-id="676fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="676fe-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="676fe-123">Authorization</span></span>|<span data-ttu-id="676fe-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="676fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="676fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="676fe-125">Accept</span></span>|<span data-ttu-id="676fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="676fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="676fe-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="676fe-127">Request body</span></span>
<span data-ttu-id="676fe-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementTroubleshootingEvent an.</span><span class="sxs-lookup"><span data-stu-id="676fe-128">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="676fe-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="676fe-129">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="676fe-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="676fe-130">Property</span></span>|<span data-ttu-id="676fe-131">Typ</span><span class="sxs-lookup"><span data-stu-id="676fe-131">Type</span></span>|<span data-ttu-id="676fe-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="676fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="676fe-133">id</span><span class="sxs-lookup"><span data-stu-id="676fe-133">id</span></span>|<span data-ttu-id="676fe-134">String</span><span class="sxs-lookup"><span data-stu-id="676fe-134">String</span></span>|<span data-ttu-id="676fe-135">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="676fe-135">UUID for the object</span></span>|
|<span data-ttu-id="676fe-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="676fe-136">eventDateTime</span></span>|<span data-ttu-id="676fe-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="676fe-137">DateTimeOffset</span></span>|<span data-ttu-id="676fe-138">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="676fe-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="676fe-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="676fe-139">correlationId</span></span>|<span data-ttu-id="676fe-140">String</span><span class="sxs-lookup"><span data-stu-id="676fe-140">String</span></span>|<span data-ttu-id="676fe-141">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="676fe-141">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="676fe-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="676fe-142">Response</span></span>
<span data-ttu-id="676fe-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="676fe-143">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="676fe-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="676fe-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="676fe-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="676fe-145">Request</span></span>
<span data-ttu-id="676fe-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="676fe-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="676fe-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="676fe-147">Response</span></span>
<span data-ttu-id="676fe-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="676fe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





