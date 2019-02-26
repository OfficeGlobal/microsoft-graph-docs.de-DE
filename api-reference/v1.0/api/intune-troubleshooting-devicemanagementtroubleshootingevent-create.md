---
title: deviceManagementTroubleshootingEvent erstellen
description: Erstellen eines neuen deviceManagementTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d222ddfa480072baefd943ca38ea8ade6d61641
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258450"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="1bdeb-103">deviceManagementTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="1bdeb-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="1bdeb-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1bdeb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bdeb-105">Erstellen eines neuen [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1bdeb-105">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bdeb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1bdeb-106">Prerequisites</span></span>
<span data-ttu-id="1bdeb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1bdeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1bdeb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1bdeb-109">Permission type</span></span>|<span data-ttu-id="1bdeb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1bdeb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bdeb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1bdeb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1bdeb-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bdeb-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1bdeb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1bdeb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bdeb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1bdeb-114">Not supported.</span></span>|
|<span data-ttu-id="1bdeb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1bdeb-115">Application</span></span>|<span data-ttu-id="1bdeb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1bdeb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bdeb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1bdeb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="1bdeb-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1bdeb-118">Request headers</span></span>
|<span data-ttu-id="1bdeb-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1bdeb-119">Header</span></span>|<span data-ttu-id="1bdeb-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1bdeb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bdeb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bdeb-121">Authorization</span></span>|<span data-ttu-id="1bdeb-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1bdeb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bdeb-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1bdeb-123">Accept</span></span>|<span data-ttu-id="1bdeb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1bdeb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bdeb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1bdeb-125">Request body</span></span>
<span data-ttu-id="1bdeb-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementTroubleshootingEvent an.</span><span class="sxs-lookup"><span data-stu-id="1bdeb-126">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="1bdeb-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="1bdeb-127">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="1bdeb-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1bdeb-128">Property</span></span>|<span data-ttu-id="1bdeb-129">Typ</span><span class="sxs-lookup"><span data-stu-id="1bdeb-129">Type</span></span>|<span data-ttu-id="1bdeb-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1bdeb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bdeb-131">id</span><span class="sxs-lookup"><span data-stu-id="1bdeb-131">id</span></span>|<span data-ttu-id="1bdeb-132">String</span><span class="sxs-lookup"><span data-stu-id="1bdeb-132">String</span></span>|<span data-ttu-id="1bdeb-133">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="1bdeb-133">UUID for the object</span></span>|
|<span data-ttu-id="1bdeb-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="1bdeb-134">eventDateTime</span></span>|<span data-ttu-id="1bdeb-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bdeb-135">DateTimeOffset</span></span>|<span data-ttu-id="1bdeb-136">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="1bdeb-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="1bdeb-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="1bdeb-137">correlationId</span></span>|<span data-ttu-id="1bdeb-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1bdeb-138">String</span></span>|<span data-ttu-id="1bdeb-139">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="1bdeb-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="1bdeb-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1bdeb-140">Response</span></span>
<span data-ttu-id="1bdeb-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1bdeb-141">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bdeb-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1bdeb-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bdeb-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1bdeb-143">Request</span></span>
<span data-ttu-id="1bdeb-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1bdeb-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1bdeb-145">Reaktion</span><span class="sxs-lookup"><span data-stu-id="1bdeb-145">Response</span></span>
<span data-ttu-id="1bdeb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1bdeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



