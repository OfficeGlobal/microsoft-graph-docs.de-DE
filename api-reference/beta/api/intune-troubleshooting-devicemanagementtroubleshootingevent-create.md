---
title: deviceManagementTroubleshootingEvent erstellen
description: Erstellen eines neuen deviceManagementTroubleshootingEvent-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f8b88d0474c7b332b91d447c963fa2a983b64035
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404428"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="c4740-103">deviceManagementTroubleshootingEvent erstellen</span><span class="sxs-lookup"><span data-stu-id="c4740-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="c4740-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c4740-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c4740-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c4740-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c4740-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c4740-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4740-107">Erstellen eines neuen [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c4740-107">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4740-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c4740-108">Prerequisites</span></span>
<span data-ttu-id="c4740-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c4740-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c4740-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c4740-111">Permission type</span></span>|<span data-ttu-id="c4740-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c4740-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4740-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c4740-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4740-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4740-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c4740-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c4740-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4740-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c4740-116">Not supported.</span></span>|
|<span data-ttu-id="c4740-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c4740-117">Application</span></span>|<span data-ttu-id="c4740-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c4740-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4740-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4740-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="c4740-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c4740-120">Request headers</span></span>
|<span data-ttu-id="c4740-121">Header</span><span class="sxs-lookup"><span data-stu-id="c4740-121">Header</span></span>|<span data-ttu-id="c4740-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c4740-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4740-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c4740-123">Authorization</span></span>|<span data-ttu-id="c4740-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c4740-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4740-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c4740-125">Accept</span></span>|<span data-ttu-id="c4740-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4740-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4740-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c4740-127">Request body</span></span>
<span data-ttu-id="c4740-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementTroubleshootingEvent an.</span><span class="sxs-lookup"><span data-stu-id="c4740-128">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="c4740-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementTroubleshootingEvent erstellen.</span><span class="sxs-lookup"><span data-stu-id="c4740-129">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="c4740-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c4740-130">Property</span></span>|<span data-ttu-id="c4740-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c4740-131">Type</span></span>|<span data-ttu-id="c4740-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4740-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4740-133">id</span><span class="sxs-lookup"><span data-stu-id="c4740-133">id</span></span>|<span data-ttu-id="c4740-134">String</span><span class="sxs-lookup"><span data-stu-id="c4740-134">String</span></span>|<span data-ttu-id="c4740-135">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="c4740-135">UUID for the object</span></span>|
|<span data-ttu-id="c4740-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="c4740-136">eventDateTime</span></span>|<span data-ttu-id="c4740-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4740-137">DateTimeOffset</span></span>|<span data-ttu-id="c4740-138">Uhrzeit, zu der das Ereignis aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="c4740-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="c4740-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="c4740-139">correlationId</span></span>|<span data-ttu-id="c4740-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4740-140">String</span></span>|<span data-ttu-id="c4740-141">ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="c4740-141">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="c4740-142">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c4740-142">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="c4740-143">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c4740-143">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="c4740-144">Enthält detaillierte Informationen zu dem Fehler und seine Remediation-Objekt.</span><span class="sxs-lookup"><span data-stu-id="c4740-144">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="c4740-145">Ereignisname</span><span class="sxs-lookup"><span data-stu-id="c4740-145">eventName</span></span>|<span data-ttu-id="c4740-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4740-146">String</span></span>|<span data-ttu-id="c4740-147">Name des Ereignisses, das Ereignis Problembehandlung entspricht.</span><span class="sxs-lookup"><span data-stu-id="c4740-147">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="c4740-148">Es ist ein optionales Feld</span><span class="sxs-lookup"><span data-stu-id="c4740-148">It is an Optional field</span></span>|
|<span data-ttu-id="c4740-149">zusätzliche Informationen</span><span class="sxs-lookup"><span data-stu-id="c4740-149">additionalInformation</span></span>|<span data-ttu-id="c4740-150">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c4740-150">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c4740-151">Eine Reihe von Schlüssel und String-Wert-Paare bietet zusätzliche Informationen für die Problembehandlung bei-Ereignis</span><span class="sxs-lookup"><span data-stu-id="c4740-151">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="c4740-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="c4740-152">Response</span></span>
<span data-ttu-id="c4740-153">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c4740-153">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4740-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c4740-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4740-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4740-155">Request</span></span>
<span data-ttu-id="c4740-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c4740-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 852

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="c4740-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="c4740-157">Response</span></span>
<span data-ttu-id="c4740-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c4740-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 901

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
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
  ]
}
```




