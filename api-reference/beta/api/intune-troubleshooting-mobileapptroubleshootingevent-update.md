---
title: MobileAppTroubleshootingEvent aktualisieren
description: Aktualisieren Sie die Eigenschaften eines MobileAppTroubleshootingEvent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ec0c30cc2c37e65fa0a6adebf0bd3a171530640d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940071"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="0be7f-103">MobileAppTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0be7f-103">Update mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="0be7f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0be7f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0be7f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0be7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0be7f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0be7f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0be7f-107">Aktualisieren Sie die Eigenschaften eines [MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0be7f-107">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0be7f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0be7f-108">Prerequisites</span></span>
<span data-ttu-id="0be7f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0be7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0be7f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0be7f-111">Permission type</span></span>|<span data-ttu-id="0be7f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0be7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0be7f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0be7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0be7f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be7f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0be7f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0be7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0be7f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0be7f-116">Not supported.</span></span>|
|<span data-ttu-id="0be7f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0be7f-117">Application</span></span>|<span data-ttu-id="0be7f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0be7f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0be7f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0be7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="0be7f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0be7f-120">Request headers</span></span>
|<span data-ttu-id="0be7f-121">Header</span><span class="sxs-lookup"><span data-stu-id="0be7f-121">Header</span></span>|<span data-ttu-id="0be7f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0be7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0be7f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0be7f-123">Authorization</span></span>|<span data-ttu-id="0be7f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0be7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0be7f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0be7f-125">Accept</span></span>|<span data-ttu-id="0be7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0be7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0be7f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0be7f-127">Request body</span></span>
<span data-ttu-id="0be7f-128">Geben Sie im Textkörper Anforderung für das Objekt [MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="0be7f-128">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="0be7f-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="0be7f-129">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="0be7f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0be7f-130">Property</span></span>|<span data-ttu-id="0be7f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0be7f-131">Type</span></span>|<span data-ttu-id="0be7f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0be7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0be7f-133">id</span><span class="sxs-lookup"><span data-stu-id="0be7f-133">id</span></span>|<span data-ttu-id="0be7f-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0be7f-134">String</span></span>|<span data-ttu-id="0be7f-135">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="0be7f-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="0be7f-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="0be7f-136">eventDateTime</span></span>|<span data-ttu-id="0be7f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0be7f-137">DateTimeOffset</span></span>|<span data-ttu-id="0be7f-138">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="0be7f-138">Time when the event occurred .</span></span> <span data-ttu-id="0be7f-139">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="0be7f-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="0be7f-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="0be7f-140">correlationId</span></span>|<span data-ttu-id="0be7f-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0be7f-141">String</span></span>|<span data-ttu-id="0be7f-142">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="0be7f-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="0be7f-143">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="0be7f-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="0be7f-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="0be7f-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="0be7f-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0be7f-145">String</span></span>|<span data-ttu-id="0be7f-146">Von Intune erstellter oder erfasster Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="0be7f-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="0be7f-147">userId</span><span class="sxs-lookup"><span data-stu-id="0be7f-147">userId</span></span>|<span data-ttu-id="0be7f-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0be7f-148">String</span></span>|<span data-ttu-id="0be7f-149">Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="0be7f-149">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="0be7f-150">applicationId</span><span class="sxs-lookup"><span data-stu-id="0be7f-150">applicationId</span></span>|<span data-ttu-id="0be7f-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0be7f-151">String</span></span>|<span data-ttu-id="0be7f-152">Intune Anwendungsbezeichner.</span><span class="sxs-lookup"><span data-stu-id="0be7f-152">Intune application identifier.</span></span>|
|<span data-ttu-id="0be7f-153">Verlauf</span><span class="sxs-lookup"><span data-stu-id="0be7f-153">history</span></span>|<span data-ttu-id="0be7f-154">[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0be7f-154">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="0be7f-155">Intune Mobile Anwendung Problembehandlung Historienelement</span><span class="sxs-lookup"><span data-stu-id="0be7f-155">Intune Mobile Application Troubleshooting History Item</span></span>|



## <a name="response"></a><span data-ttu-id="0be7f-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="0be7f-156">Response</span></span>
<span data-ttu-id="0be7f-157">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0be7f-157">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0be7f-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0be7f-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="0be7f-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0be7f-159">Request</span></span>
<span data-ttu-id="0be7f-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0be7f-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 421

{
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

### <a name="response"></a><span data-ttu-id="0be7f-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="0be7f-161">Response</span></span>
<span data-ttu-id="0be7f-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0be7f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





