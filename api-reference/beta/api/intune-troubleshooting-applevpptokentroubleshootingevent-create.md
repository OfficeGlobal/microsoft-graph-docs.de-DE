---
title: Erstellen von appleVppTokenTroubleshootingEvent
description: Erstellen eines neuen AppleVppTokenTroubleshootingEvent-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a2db5607059ca16d1b1df00f4f0f21d7233ab6db
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431534"
---
# <a name="create-applevpptokentroubleshootingevent"></a><span data-ttu-id="f8b44-103">Erstellen von appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f8b44-103">Create appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="f8b44-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f8b44-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f8b44-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8b44-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8b44-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f8b44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8b44-107">Erstellen eines neuen [AppleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f8b44-107">Create a new [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8b44-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f8b44-108">Prerequisites</span></span>
<span data-ttu-id="f8b44-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f8b44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f8b44-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8b44-111">Permission type</span></span>|<span data-ttu-id="f8b44-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8b44-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8b44-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8b44-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8b44-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8b44-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f8b44-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8b44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8b44-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8b44-116">Not supported.</span></span>|
|<span data-ttu-id="f8b44-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8b44-117">Application</span></span>|<span data-ttu-id="f8b44-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8b44-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8b44-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8b44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="f8b44-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8b44-120">Request headers</span></span>
|<span data-ttu-id="f8b44-121">Header</span><span class="sxs-lookup"><span data-stu-id="f8b44-121">Header</span></span>|<span data-ttu-id="f8b44-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f8b44-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8b44-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f8b44-123">Authorization</span></span>|<span data-ttu-id="f8b44-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f8b44-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8b44-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f8b44-125">Accept</span></span>|<span data-ttu-id="f8b44-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8b44-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8b44-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f8b44-127">Request body</span></span>
<span data-ttu-id="f8b44-128">Geben Sie im Textkörper Anforderung für das Objekt AppleVppTokenTroubleshootingEvent eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f8b44-128">In the request body, supply a JSON representation for the appleVppTokenTroubleshootingEvent object.</span></span>

<span data-ttu-id="f8b44-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AppleVppTokenTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="f8b44-129">The following table shows the properties that are required when you create the appleVppTokenTroubleshootingEvent.</span></span>

|<span data-ttu-id="f8b44-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8b44-130">Property</span></span>|<span data-ttu-id="f8b44-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f8b44-131">Type</span></span>|<span data-ttu-id="f8b44-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8b44-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8b44-133">id</span><span class="sxs-lookup"><span data-stu-id="f8b44-133">id</span></span>|<span data-ttu-id="f8b44-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8b44-134">String</span></span>|<span data-ttu-id="f8b44-135">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f8b44-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f8b44-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="f8b44-136">eventDateTime</span></span>|<span data-ttu-id="f8b44-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8b44-137">DateTimeOffset</span></span>|<span data-ttu-id="f8b44-138">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="f8b44-138">Time when the event occurred .</span></span> <span data-ttu-id="f8b44-139">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f8b44-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f8b44-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="f8b44-140">correlationId</span></span>|<span data-ttu-id="f8b44-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8b44-141">String</span></span>|<span data-ttu-id="f8b44-142">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="f8b44-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="f8b44-143">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f8b44-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f8b44-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f8b44-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="f8b44-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f8b44-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="f8b44-146">Enthält detaillierte Informationen zu dem Fehler und seine Remediation-Objekt.</span><span class="sxs-lookup"><span data-stu-id="f8b44-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="f8b44-147">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f8b44-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f8b44-148">Ereignisname</span><span class="sxs-lookup"><span data-stu-id="f8b44-148">eventName</span></span>|<span data-ttu-id="f8b44-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8b44-149">String</span></span>|<span data-ttu-id="f8b44-150">Name des Ereignisses, das Ereignis Problembehandlung entspricht.</span><span class="sxs-lookup"><span data-stu-id="f8b44-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="f8b44-151">Es ist ein optionales Feld Inherited aus [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f8b44-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f8b44-152">zusätzliche Informationen</span><span class="sxs-lookup"><span data-stu-id="f8b44-152">additionalInformation</span></span>|<span data-ttu-id="f8b44-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f8b44-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f8b44-154">Eine Reihe von Schlüssel und String-Wert-Paare bietet zusätzliche Informationen für die Problembehandlung bei Ereignis Inherited aus [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="f8b44-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="f8b44-155">tokenId</span><span class="sxs-lookup"><span data-stu-id="f8b44-155">tokenId</span></span>|<span data-ttu-id="f8b44-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8b44-156">String</span></span>|<span data-ttu-id="f8b44-157">Apple Volume Purchase Programm Token-ID.</span><span class="sxs-lookup"><span data-stu-id="f8b44-157">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="f8b44-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8b44-158">Response</span></span>
<span data-ttu-id="f8b44-159">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AppleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f8b44-159">If successful, this method returns a `201 Created` response code and a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8b44-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f8b44-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8b44-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8b44-161">Request</span></span>
<span data-ttu-id="f8b44-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8b44-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 881

{
  "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "tokenId": "Token Id value"
}
```

### <a name="response"></a><span data-ttu-id="f8b44-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8b44-163">Response</span></span>
<span data-ttu-id="f8b44-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8b44-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 930

{
  "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
  "id": "09295f26-5f26-0929-265f-2909265f2909",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "tokenId": "Token Id value"
}
```




