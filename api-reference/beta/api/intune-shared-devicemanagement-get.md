---
title: deviceManagement abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceManagement-Objekts.
ms.openlocfilehash: adc45ed789e3e636282fee851997c3fbcc8d8318
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061430"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="97a68-103">deviceManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="97a68-103">Get deviceManagement</span></span>

> <span data-ttu-id="97a68-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="97a68-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97a68-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97a68-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97a68-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="97a68-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97a68-107">Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="97a68-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97a68-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="97a68-108">Prerequisites</span></span>

<span data-ttu-id="97a68-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97a68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97a68-111">Berechtigung&nbsp;Typ&nbsp;(durch&nbsp;Workflow)</span><span class="sxs-lookup"><span data-stu-id="97a68-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="97a68-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97a68-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="97a68-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97a68-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="97a68-114">&nbsp;&nbsp; **Für die Arbeit android**</span><span class="sxs-lookup"><span data-stu-id="97a68-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="97a68-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="97a68-116">&nbsp; &nbsp; **Überwachung**</span><span class="sxs-lookup"><span data-stu-id="97a68-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="97a68-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="97a68-118">&nbsp;&nbsp; **Unternehmen Begriffe**</span><span class="sxs-lookup"><span data-stu-id="97a68-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="97a68-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="97a68-120">&nbsp;&nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="97a68-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="97a68-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="97a68-122">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="97a68-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="97a68-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="97a68-124">&nbsp;&nbsp; **Elektronische SIM**</span><span class="sxs-lookup"><span data-stu-id="97a68-124">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="97a68-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="97a68-126">&nbsp; &nbsp; **Registrierung**</span><span class="sxs-lookup"><span data-stu-id="97a68-126">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="97a68-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="97a68-128">&nbsp;&nbsp; **Zauns**</span><span class="sxs-lookup"><span data-stu-id="97a68-128">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="97a68-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="97a68-130">&nbsp;&nbsp; **Benachrichtigung**</span><span class="sxs-lookup"><span data-stu-id="97a68-130">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="97a68-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="97a68-132">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="97a68-132">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="97a68-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="97a68-134">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="97a68-134">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="97a68-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="97a68-136">&nbsp;&nbsp; **Remotezugriff**</span><span class="sxs-lookup"><span data-stu-id="97a68-136">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="97a68-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="97a68-138">&nbsp;&nbsp; **Remoteunterstützung**</span><span class="sxs-lookup"><span data-stu-id="97a68-138">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="97a68-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="97a68-140">&nbsp;&nbsp; **Telekommunikation Ausgaben Management**</span><span class="sxs-lookup"><span data-stu-id="97a68-140">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="97a68-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="97a68-142">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="97a68-142">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="97a68-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="97a68-144">&nbsp;&nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="97a68-144">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="97a68-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="97a68-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="97a68-146">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97a68-146">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97a68-147">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97a68-147">Not supported.</span></span>|
| <span data-ttu-id="97a68-148">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97a68-148">Application</span></span> | <span data-ttu-id="97a68-149">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97a68-149">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="97a68-150">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97a68-150">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="97a68-151">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="97a68-151">Optional query parameters</span></span>

<span data-ttu-id="97a68-152">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="97a68-152">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97a68-153">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97a68-153">Request headers</span></span>
|<span data-ttu-id="97a68-154">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="97a68-154">Header</span></span>|<span data-ttu-id="97a68-155">Wert</span><span class="sxs-lookup"><span data-stu-id="97a68-155">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97a68-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="97a68-156">Authorization</span></span>|<span data-ttu-id="97a68-157">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="97a68-157">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97a68-158">Accept</span><span class="sxs-lookup"><span data-stu-id="97a68-158">Accept</span></span>|<span data-ttu-id="97a68-159">application/json</span><span class="sxs-lookup"><span data-stu-id="97a68-159">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97a68-160">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97a68-160">Request body</span></span>

<span data-ttu-id="97a68-161">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="97a68-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97a68-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="97a68-162">Response</span></span>

<span data-ttu-id="97a68-163">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="97a68-163">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97a68-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97a68-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="97a68-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97a68-165">Request</span></span>

<span data-ttu-id="97a68-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97a68-166">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="97a68-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="97a68-167">Response</span></span>

<span data-ttu-id="97a68-168">Hier einige Beispiele der Antwort.</span><span class="sxs-lookup"><span data-stu-id="97a68-168">Here are example of the response.</span></span> 

<span data-ttu-id="97a68-169">Hinweis: Die hier gezeigte Antwortobjekte der Kürze halber werden möglicherweise abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="97a68-169">Note: The response objects shown here may be truncated for brevity.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

<span data-ttu-id="97a68-170">Eigenschaften für den Workflow entsprechenden werden zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97a68-170">Properties appropriate for the workflow are returned.</span></span>

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



