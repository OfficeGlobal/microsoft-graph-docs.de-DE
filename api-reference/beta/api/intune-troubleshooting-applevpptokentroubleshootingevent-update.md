---
title: AppleVppTokenTroubleshootingEvent aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AppleVppTokenTroubleshootingEvent-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3382eb7069be27fb47bf094d4a0688d7cd128de6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430036"
---
# <a name="update-applevpptokentroubleshootingevent"></a><span data-ttu-id="cfff2-103">AppleVppTokenTroubleshootingEvent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="cfff2-103">Update appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="cfff2-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="cfff2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cfff2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cfff2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cfff2-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cfff2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfff2-107">Aktualisieren Sie die Eigenschaften eines [AppleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="cfff2-107">Update the properties of a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfff2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cfff2-108">Prerequisites</span></span>
<span data-ttu-id="cfff2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cfff2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cfff2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cfff2-111">Permission type</span></span>|<span data-ttu-id="cfff2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cfff2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfff2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cfff2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cfff2-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfff2-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cfff2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cfff2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfff2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cfff2-116">Not supported.</span></span>|
|<span data-ttu-id="cfff2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cfff2-117">Application</span></span>|<span data-ttu-id="cfff2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cfff2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfff2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cfff2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="cfff2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cfff2-120">Request headers</span></span>
|<span data-ttu-id="cfff2-121">Header</span><span class="sxs-lookup"><span data-stu-id="cfff2-121">Header</span></span>|<span data-ttu-id="cfff2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="cfff2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfff2-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cfff2-123">Authorization</span></span>|<span data-ttu-id="cfff2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cfff2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfff2-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cfff2-125">Accept</span></span>|<span data-ttu-id="cfff2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cfff2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfff2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cfff2-127">Request body</span></span>
<span data-ttu-id="cfff2-128">Geben Sie im Textkörper Anforderung für das Objekt [AppleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="cfff2-128">In the request body, supply a JSON representation for the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

<span data-ttu-id="cfff2-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AppleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="cfff2-129">The following table shows the properties that are required when you create the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span></span>

|<span data-ttu-id="cfff2-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cfff2-130">Property</span></span>|<span data-ttu-id="cfff2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="cfff2-131">Type</span></span>|<span data-ttu-id="cfff2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cfff2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfff2-133">id</span><span class="sxs-lookup"><span data-stu-id="cfff2-133">id</span></span>|<span data-ttu-id="cfff2-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cfff2-134">String</span></span>|<span data-ttu-id="cfff2-135">UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="cfff2-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="cfff2-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="cfff2-136">eventDateTime</span></span>|<span data-ttu-id="cfff2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfff2-137">DateTimeOffset</span></span>|<span data-ttu-id="cfff2-138">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="cfff2-138">Time when the event occurred .</span></span> <span data-ttu-id="cfff2-139">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="cfff2-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="cfff2-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="cfff2-140">correlationId</span></span>|<span data-ttu-id="cfff2-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cfff2-141">String</span></span>|<span data-ttu-id="cfff2-142">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="cfff2-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="cfff2-143">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="cfff2-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="cfff2-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="cfff2-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="cfff2-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="cfff2-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="cfff2-146">Enthält detaillierte Informationen zu dem Fehler und seine Remediation-Objekt.</span><span class="sxs-lookup"><span data-stu-id="cfff2-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="cfff2-147">Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="cfff2-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="cfff2-148">Ereignisname</span><span class="sxs-lookup"><span data-stu-id="cfff2-148">eventName</span></span>|<span data-ttu-id="cfff2-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cfff2-149">String</span></span>|<span data-ttu-id="cfff2-150">Name des Ereignisses, das Ereignis Problembehandlung entspricht.</span><span class="sxs-lookup"><span data-stu-id="cfff2-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="cfff2-151">Es ist ein optionales Feld Inherited aus [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="cfff2-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="cfff2-152">zusätzliche Informationen</span><span class="sxs-lookup"><span data-stu-id="cfff2-152">additionalInformation</span></span>|<span data-ttu-id="cfff2-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="cfff2-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="cfff2-154">Eine Reihe von Schlüssel und String-Wert-Paare bietet zusätzliche Informationen für die Problembehandlung bei Ereignis Inherited aus [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="cfff2-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="cfff2-155">tokenId</span><span class="sxs-lookup"><span data-stu-id="cfff2-155">tokenId</span></span>|<span data-ttu-id="cfff2-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cfff2-156">String</span></span>|<span data-ttu-id="cfff2-157">Apple Volume Purchase Programm Token-ID.</span><span class="sxs-lookup"><span data-stu-id="cfff2-157">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="cfff2-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="cfff2-158">Response</span></span>
<span data-ttu-id="cfff2-159">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AppleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="cfff2-159">If successful, this method returns a `200 OK` response code and an updated [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfff2-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cfff2-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfff2-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cfff2-161">Request</span></span>
<span data-ttu-id="cfff2-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cfff2-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
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

### <a name="response"></a><span data-ttu-id="cfff2-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="cfff2-163">Response</span></span>
<span data-ttu-id="cfff2-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cfff2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




