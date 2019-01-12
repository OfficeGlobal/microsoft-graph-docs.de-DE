---
title: deviceManagement abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceManagement-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: af4dc08832b09387774ad3ad1642b0103b3b7db9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936928"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="45ec8-103">deviceManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="45ec8-103">Get deviceManagement</span></span>

> <span data-ttu-id="45ec8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="45ec8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45ec8-105">Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="45ec8-105">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45ec8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="45ec8-106">Prerequisites</span></span>
<span data-ttu-id="45ec8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45ec8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="45ec8-109">Berechtigung&nbsp;Typ&nbsp;(durch&nbsp;Workflow)</span><span class="sxs-lookup"><span data-stu-id="45ec8-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="45ec8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="45ec8-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="45ec8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="45ec8-111">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="45ec8-112">&nbsp;&nbsp; Überwachung</span><span class="sxs-lookup"><span data-stu-id="45ec8-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="45ec8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ec8-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="45ec8-114">&nbsp;&nbsp; Begriffe des Unternehmens</span><span class="sxs-lookup"><span data-stu-id="45ec8-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="45ec8-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ec8-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="45ec8-116">&nbsp;&nbsp; Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="45ec8-116">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="45ec8-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ec8-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="45ec8-118">&nbsp;&nbsp; Gerätemanagement</span><span class="sxs-lookup"><span data-stu-id="45ec8-118">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="45ec8-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ec8-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="45ec8-120">&nbsp;&nbsp; Registrierung</span><span class="sxs-lookup"><span data-stu-id="45ec8-120">&nbsp; &nbsp; Enrollment</span></span> | <span data-ttu-id="45ec8-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ec8-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="45ec8-122">&nbsp;&nbsp; Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="45ec8-122">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="45ec8-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ec8-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="45ec8-124">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="45ec8-124">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="45ec8-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ec8-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="45ec8-126">&nbsp;&nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="45ec8-126">&nbsp; &nbsp; RBAC</span></span> | <span data-ttu-id="45ec8-127">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ec8-127">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="45ec8-128">&nbsp;&nbsp; Remoteunterstützung</span><span class="sxs-lookup"><span data-stu-id="45ec8-128">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="45ec8-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ec8-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="45ec8-130">&nbsp;&nbsp; Telekommunikation Ausgaben Management</span><span class="sxs-lookup"><span data-stu-id="45ec8-130">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="45ec8-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ec8-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="45ec8-132">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="45ec8-132">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="45ec8-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ec8-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="45ec8-134">&nbsp;&nbsp; Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="45ec8-134">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="45ec8-135">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ec8-135">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="45ec8-136">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="45ec8-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45ec8-137">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45ec8-137">Not supported.</span></span>|
| <span data-ttu-id="45ec8-138">Anwendung</span><span class="sxs-lookup"><span data-stu-id="45ec8-138">Application</span></span> | <span data-ttu-id="45ec8-139">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45ec8-139">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="45ec8-140">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="45ec8-140">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45ec8-141">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="45ec8-141">Optional query parameters</span></span>
<span data-ttu-id="45ec8-142">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="45ec8-142">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="45ec8-143">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="45ec8-143">Request headers</span></span>
|<span data-ttu-id="45ec8-144">Header</span><span class="sxs-lookup"><span data-stu-id="45ec8-144">Header</span></span>|<span data-ttu-id="45ec8-145">Wert</span><span class="sxs-lookup"><span data-stu-id="45ec8-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45ec8-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="45ec8-146">Authorization</span></span>|<span data-ttu-id="45ec8-147">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="45ec8-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45ec8-148">Annehmen</span><span class="sxs-lookup"><span data-stu-id="45ec8-148">Accept</span></span>|<span data-ttu-id="45ec8-149">application/json</span><span class="sxs-lookup"><span data-stu-id="45ec8-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45ec8-150">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="45ec8-150">Request body</span></span>
<span data-ttu-id="45ec8-151">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="45ec8-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45ec8-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="45ec8-152">Response</span></span>
<span data-ttu-id="45ec8-153">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="45ec8-153">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45ec8-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="45ec8-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="45ec8-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="45ec8-155">Request</span></span>
<span data-ttu-id="45ec8-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="45ec8-156">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="45ec8-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="45ec8-157">Response</span></span>
<span data-ttu-id="45ec8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="45ec8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b",
    "subscriptionState": "active",
    "subscriptions": "intune",
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent",
      "shareAPNSData": "granted"
    },
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview",
      "totalReportedDeviceCount": 8,
      "inactiveThreatAgentDeviceCount": 14,
      "unknownStateThreatAgentDeviceCount": 2,
      "pendingSignatureUpdateDeviceCount": 1,
      "cleanDeviceCount": 0,
      "pendingFullScanDeviceCount": 10,
      "pendingRestartDeviceCount": 9,
      "pendingManualStepsDeviceCount": 13,
      "pendingOfflineScanDeviceCount": 13,
      "criticalFailuresDeviceCount": 11
    },
    "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
  }
}
```



