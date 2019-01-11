---
title: deviceManagementTroubleshootingEvent erstellen
description: Erstellen eines neuen deviceManagementTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 25253b9851c675417801b41692ffaa90a1fe1039
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851779"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="0cf41-103">deviceManagementTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="0cf41-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="0cf41-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0cf41-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0cf41-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0cf41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0cf41-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0cf41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0cf41-107">Erstellen eines neuen [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0cf41-107">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0cf41-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0cf41-108">Prerequisites</span></span>
<span data-ttu-id="0cf41-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cf41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cf41-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0cf41-111">Permission type</span></span>|<span data-ttu-id="0cf41-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0cf41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cf41-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0cf41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0cf41-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cf41-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0cf41-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0cf41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cf41-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0cf41-116">Not supported.</span></span>|
|<span data-ttu-id="0cf41-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0cf41-117">Application</span></span>|<span data-ttu-id="0cf41-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0cf41-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cf41-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0cf41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="0cf41-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0cf41-120">Request headers</span></span>
|<span data-ttu-id="0cf41-121">Header</span><span class="sxs-lookup"><span data-stu-id="0cf41-121">Header</span></span>|<span data-ttu-id="0cf41-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0cf41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cf41-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cf41-123">Authorization</span></span>|<span data-ttu-id="0cf41-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0cf41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cf41-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0cf41-125">Accept</span></span>|<span data-ttu-id="0cf41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0cf41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cf41-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0cf41-127">Request body</span></span>
<span data-ttu-id="0cf41-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementTroubleshootingEvent an.</span><span class="sxs-lookup"><span data-stu-id="0cf41-128">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="0cf41-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="0cf41-129">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="0cf41-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0cf41-130">Property</span></span>|<span data-ttu-id="0cf41-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0cf41-131">Type</span></span>|<span data-ttu-id="0cf41-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0cf41-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cf41-133">id</span><span class="sxs-lookup"><span data-stu-id="0cf41-133">id</span></span>|<span data-ttu-id="0cf41-134">String</span><span class="sxs-lookup"><span data-stu-id="0cf41-134">String</span></span>|<span data-ttu-id="0cf41-135">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="0cf41-135">UUID for the object</span></span>|
|<span data-ttu-id="0cf41-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="0cf41-136">eventDateTime</span></span>|<span data-ttu-id="0cf41-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cf41-137">DateTimeOffset</span></span>|<span data-ttu-id="0cf41-138">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="0cf41-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="0cf41-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="0cf41-139">correlationId</span></span>|<span data-ttu-id="0cf41-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0cf41-140">String</span></span>|<span data-ttu-id="0cf41-141">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="0cf41-141">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="0cf41-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="0cf41-142">Response</span></span>
<span data-ttu-id="0cf41-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0cf41-143">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cf41-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0cf41-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="0cf41-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0cf41-145">Request</span></span>
<span data-ttu-id="0cf41-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0cf41-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0cf41-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="0cf41-147">Response</span></span>
<span data-ttu-id="0cf41-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0cf41-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





