---
title: deviceManagement abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceManagement-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7ae3300ffa73aa42481930e5701755d2551a6076
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250635"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="20b87-103">deviceManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="20b87-103">Get deviceManagement</span></span>

> <span data-ttu-id="20b87-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="20b87-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20b87-105">Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="20b87-105">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20b87-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="20b87-106">Prerequisites</span></span>
<span data-ttu-id="20b87-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20b87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20b87-109">&nbsp;Berechtigungstyp&nbsp;(nach&nbsp;Workflow)</span><span class="sxs-lookup"><span data-stu-id="20b87-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="20b87-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="20b87-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="20b87-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="20b87-111">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="20b87-112">&nbsp;&nbsp; Überwachung</span><span class="sxs-lookup"><span data-stu-id="20b87-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="20b87-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b87-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="20b87-114">&nbsp;&nbsp; Unternehmensbedingungen</span><span class="sxs-lookup"><span data-stu-id="20b87-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="20b87-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b87-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="20b87-116">&nbsp;&nbsp; Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="20b87-116">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="20b87-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b87-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="20b87-118">&nbsp;&nbsp; Geräteverwaltung</span><span class="sxs-lookup"><span data-stu-id="20b87-118">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="20b87-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b87-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="20b87-120">&nbsp;&nbsp; Registrierung</span><span class="sxs-lookup"><span data-stu-id="20b87-120">&nbsp; &nbsp; Enrollment</span></span> | <span data-ttu-id="20b87-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b87-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="20b87-122">&nbsp;&nbsp; Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="20b87-122">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="20b87-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b87-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="20b87-124">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="20b87-124">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="20b87-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b87-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="20b87-126">&nbsp;&nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="20b87-126">&nbsp; &nbsp; RBAC</span></span> | <span data-ttu-id="20b87-127">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b87-127">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="20b87-128">&nbsp;&nbsp; Remote Unterstützung</span><span class="sxs-lookup"><span data-stu-id="20b87-128">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="20b87-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b87-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="20b87-130">&nbsp;&nbsp; Telekom-Spesenverwaltung</span><span class="sxs-lookup"><span data-stu-id="20b87-130">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="20b87-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b87-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="20b87-132">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="20b87-132">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="20b87-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b87-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="20b87-134">&nbsp;&nbsp; Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="20b87-134">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="20b87-135">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b87-135">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="20b87-136">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="20b87-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20b87-137">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="20b87-137">Not supported.</span></span>|
| <span data-ttu-id="20b87-138">Anwendung</span><span class="sxs-lookup"><span data-stu-id="20b87-138">Application</span></span> | <span data-ttu-id="20b87-139">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="20b87-139">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="20b87-140">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="20b87-140">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20b87-141">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="20b87-141">Optional query parameters</span></span>
<span data-ttu-id="20b87-142">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="20b87-142">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="20b87-143">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="20b87-143">Request headers</span></span>
|<span data-ttu-id="20b87-144">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="20b87-144">Header</span></span>|<span data-ttu-id="20b87-145">Wert</span><span class="sxs-lookup"><span data-stu-id="20b87-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20b87-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="20b87-146">Authorization</span></span>|<span data-ttu-id="20b87-147">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="20b87-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20b87-148">Annehmen</span><span class="sxs-lookup"><span data-stu-id="20b87-148">Accept</span></span>|<span data-ttu-id="20b87-149">application/json</span><span class="sxs-lookup"><span data-stu-id="20b87-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20b87-150">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="20b87-150">Request body</span></span>
<span data-ttu-id="20b87-151">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="20b87-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20b87-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="20b87-152">Response</span></span>
<span data-ttu-id="20b87-153">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="20b87-153">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20b87-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="20b87-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="20b87-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="20b87-155">Request</span></span>
<span data-ttu-id="20b87-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="20b87-156">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="20b87-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="20b87-157">Response</span></span>
<span data-ttu-id="20b87-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="20b87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



