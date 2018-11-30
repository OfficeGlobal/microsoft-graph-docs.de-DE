---
title: deviceManagementTroubleshootingEvent erstellen
description: Erstellen eines neuen deviceManagementTroubleshootingEvent-Objekts.
ms.openlocfilehash: d1fef87009c0797511adef5204cbc5ab4d99c291
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064147"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="492d7-103">deviceManagementTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="492d7-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="492d7-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="492d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="492d7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="492d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="492d7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="492d7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="492d7-107">Erstellen eines neuen [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="492d7-107">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="492d7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="492d7-108">Prerequisites</span></span>
<span data-ttu-id="492d7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="492d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="492d7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="492d7-111">Permission type</span></span>|<span data-ttu-id="492d7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="492d7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="492d7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="492d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="492d7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="492d7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="492d7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="492d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="492d7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="492d7-116">Not supported.</span></span>|
|<span data-ttu-id="492d7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="492d7-117">Application</span></span>|<span data-ttu-id="492d7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="492d7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="492d7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="492d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="492d7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="492d7-120">Request headers</span></span>
|<span data-ttu-id="492d7-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="492d7-121">Header</span></span>|<span data-ttu-id="492d7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="492d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="492d7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="492d7-123">Authorization</span></span>|<span data-ttu-id="492d7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="492d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="492d7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="492d7-125">Accept</span></span>|<span data-ttu-id="492d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="492d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="492d7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="492d7-127">Request body</span></span>
<span data-ttu-id="492d7-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementTroubleshootingEvent an.</span><span class="sxs-lookup"><span data-stu-id="492d7-128">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="492d7-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="492d7-129">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="492d7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="492d7-130">Property</span></span>|<span data-ttu-id="492d7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="492d7-131">Type</span></span>|<span data-ttu-id="492d7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="492d7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="492d7-133">id</span><span class="sxs-lookup"><span data-stu-id="492d7-133">id</span></span>|<span data-ttu-id="492d7-134">String</span><span class="sxs-lookup"><span data-stu-id="492d7-134">String</span></span>|<span data-ttu-id="492d7-135">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="492d7-135">UUID for the object</span></span>|
|<span data-ttu-id="492d7-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="492d7-136">eventDateTime</span></span>|<span data-ttu-id="492d7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="492d7-137">DateTimeOffset</span></span>|<span data-ttu-id="492d7-138">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="492d7-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="492d7-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="492d7-139">correlationId</span></span>|<span data-ttu-id="492d7-140">String</span><span class="sxs-lookup"><span data-stu-id="492d7-140">String</span></span>|<span data-ttu-id="492d7-141">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="492d7-141">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="492d7-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="492d7-142">Response</span></span>
<span data-ttu-id="492d7-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="492d7-143">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="492d7-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="492d7-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="492d7-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="492d7-145">Request</span></span>
<span data-ttu-id="492d7-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="492d7-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="492d7-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="492d7-147">Response</span></span>
<span data-ttu-id="492d7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="492d7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





