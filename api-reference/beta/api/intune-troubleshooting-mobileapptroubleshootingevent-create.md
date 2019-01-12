---
title: Erstellen von mobileAppTroubleshootingEvent
description: Erstellen eines neuen MobileAppTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 59eea166285f55de32df2728f9bbc834e0eecac8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978144"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="4f889-103">Erstellen von mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="4f889-103">Create mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="4f889-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4f889-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f889-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4f889-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f889-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4f889-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f889-107">Erstellen eines neuen [MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4f889-107">Create a new [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f889-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4f889-108">Prerequisites</span></span>
<span data-ttu-id="4f889-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f889-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f889-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4f889-111">Permission type</span></span>|<span data-ttu-id="4f889-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4f889-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f889-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4f889-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f889-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f889-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4f889-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4f889-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f889-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4f889-116">Not supported.</span></span>|
|<span data-ttu-id="4f889-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4f889-117">Application</span></span>|<span data-ttu-id="4f889-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4f889-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f889-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f889-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="4f889-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4f889-120">Request headers</span></span>
|<span data-ttu-id="4f889-121">Header</span><span class="sxs-lookup"><span data-stu-id="4f889-121">Header</span></span>|<span data-ttu-id="4f889-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4f889-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f889-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f889-123">Authorization</span></span>|<span data-ttu-id="4f889-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4f889-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f889-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4f889-125">Accept</span></span>|<span data-ttu-id="4f889-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f889-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f889-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4f889-127">Request body</span></span>
<span data-ttu-id="4f889-128">Geben Sie im Textkörper Anforderung für das Objekt MobileAppTroubleshootingEvent eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="4f889-128">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="4f889-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die MobileAppTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="4f889-129">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="4f889-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4f889-130">Property</span></span>|<span data-ttu-id="4f889-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4f889-131">Type</span></span>|<span data-ttu-id="4f889-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f889-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f889-133">id</span><span class="sxs-lookup"><span data-stu-id="4f889-133">id</span></span>|<span data-ttu-id="4f889-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f889-134">String</span></span>|<span data-ttu-id="4f889-135">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="4f889-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="4f889-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="4f889-136">eventDateTime</span></span>|<span data-ttu-id="4f889-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f889-137">DateTimeOffset</span></span>|<span data-ttu-id="4f889-138">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="4f889-138">Time when the event occurred .</span></span> <span data-ttu-id="4f889-139">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="4f889-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="4f889-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="4f889-140">correlationId</span></span>|<span data-ttu-id="4f889-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f889-141">String</span></span>|<span data-ttu-id="4f889-142">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="4f889-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="4f889-143">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="4f889-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="4f889-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4f889-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="4f889-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f889-145">String</span></span>|<span data-ttu-id="4f889-146">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="4f889-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="4f889-147">userId</span><span class="sxs-lookup"><span data-stu-id="4f889-147">userId</span></span>|<span data-ttu-id="4f889-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f889-148">String</span></span>|<span data-ttu-id="4f889-149">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="4f889-149">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="4f889-150">applicationId</span><span class="sxs-lookup"><span data-stu-id="4f889-150">applicationId</span></span>|<span data-ttu-id="4f889-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f889-151">String</span></span>|<span data-ttu-id="4f889-152">Intune Anwendungsbezeichner.</span><span class="sxs-lookup"><span data-stu-id="4f889-152">Intune application identifier.</span></span>|
|<span data-ttu-id="4f889-153">Verlauf</span><span class="sxs-lookup"><span data-stu-id="4f889-153">history</span></span>|<span data-ttu-id="4f889-154">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4f889-154">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="4f889-155">Intune Mobile Anwendung Problembehandlung Historienelement</span><span class="sxs-lookup"><span data-stu-id="4f889-155">Intune Mobile Application Troubleshooting History Item</span></span>|



## <a name="response"></a><span data-ttu-id="4f889-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f889-156">Response</span></span>
<span data-ttu-id="4f889-157">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4f889-157">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f889-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4f889-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f889-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f889-159">Request</span></span>
<span data-ttu-id="4f889-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4f889-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 489

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "applicationId": "Application Id value",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "2017-01-01T00:03:20.8380798-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4f889-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f889-161">Response</span></span>
<span data-ttu-id="4f889-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f889-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 538

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "applicationId": "Application Id value",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "2017-01-01T00:03:20.8380798-08:00"
    }
  ]
}
```





