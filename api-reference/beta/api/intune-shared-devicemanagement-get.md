---
title: deviceManagement abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceManagement-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e4a07c2645686722c59e45f039aacb9dc3627a5d
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570619"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="833a0-103">deviceManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="833a0-103">Get deviceManagement</span></span>

> <span data-ttu-id="833a0-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="833a0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="833a0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="833a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="833a0-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="833a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="833a0-107">Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="833a0-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="833a0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="833a0-108">Prerequisites</span></span>

<span data-ttu-id="833a0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="833a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

| <span data-ttu-id="833a0-111">&nbsp;Berechtigungstyp&nbsp;(nach&nbsp;Workflow)</span><span class="sxs-lookup"><span data-stu-id="833a0-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="833a0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="833a0-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="833a0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="833a0-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="833a0-114">&nbsp;&nbsp; **Android for Work**</span><span class="sxs-lookup"><span data-stu-id="833a0-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="833a0-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="833a0-116">&nbsp; &nbsp; **Überwachung**</span><span class="sxs-lookup"><span data-stu-id="833a0-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="833a0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="833a0-118">&nbsp; &nbsp; **Geschäftsbedingungen des Unternehmens**</span><span class="sxs-lookup"><span data-stu-id="833a0-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="833a0-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="833a0-120">&nbsp; &nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="833a0-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="833a0-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="833a0-122">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="833a0-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="833a0-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="833a0-124">&nbsp;&nbsp; **Elektronische SIM-Karte**</span><span class="sxs-lookup"><span data-stu-id="833a0-124">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="833a0-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="833a0-126">&nbsp;&nbsp; **Registrierung**</span><span class="sxs-lookup"><span data-stu-id="833a0-126">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="833a0-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="833a0-128">&nbsp;&nbsp; **Fechten**</span><span class="sxs-lookup"><span data-stu-id="833a0-128">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="833a0-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="833a0-130">&nbsp; &nbsp; **Benachrichtigung**</span><span class="sxs-lookup"><span data-stu-id="833a0-130">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="833a0-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="833a0-132">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="833a0-132">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="833a0-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="833a0-134">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="833a0-134">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="833a0-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="833a0-136">&nbsp; &nbsp; **Remotezugriff**</span><span class="sxs-lookup"><span data-stu-id="833a0-136">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="833a0-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="833a0-138">&nbsp;&nbsp; **Remote Unterstützung**</span><span class="sxs-lookup"><span data-stu-id="833a0-138">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="833a0-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="833a0-140">&nbsp;&nbsp; **Telekom-Spesenverwaltung**</span><span class="sxs-lookup"><span data-stu-id="833a0-140">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="833a0-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="833a0-142">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="833a0-142">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="833a0-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="833a0-144">&nbsp;&nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="833a0-144">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="833a0-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="833a0-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="833a0-146">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="833a0-146">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="833a0-147">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="833a0-147">Not supported.</span></span>|
| <span data-ttu-id="833a0-148">Anwendung</span><span class="sxs-lookup"><span data-stu-id="833a0-148">Application</span></span> | <span data-ttu-id="833a0-149">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="833a0-149">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="833a0-150">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="833a0-150">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="833a0-151">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="833a0-151">Optional query parameters</span></span>

<span data-ttu-id="833a0-152">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="833a0-152">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="833a0-153">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="833a0-153">Request headers</span></span>
|<span data-ttu-id="833a0-154">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="833a0-154">Header</span></span>|<span data-ttu-id="833a0-155">Wert</span><span class="sxs-lookup"><span data-stu-id="833a0-155">Value</span></span>|
|:---|:---|
|<span data-ttu-id="833a0-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="833a0-156">Authorization</span></span>|<span data-ttu-id="833a0-157">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="833a0-157">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="833a0-158">Annehmen</span><span class="sxs-lookup"><span data-stu-id="833a0-158">Accept</span></span>|<span data-ttu-id="833a0-159">application/json</span><span class="sxs-lookup"><span data-stu-id="833a0-159">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="833a0-160">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="833a0-160">Request body</span></span>

<span data-ttu-id="833a0-161">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="833a0-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="833a0-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="833a0-162">Response</span></span>

<span data-ttu-id="833a0-163">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="833a0-163">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="833a0-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="833a0-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="833a0-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="833a0-165">Request</span></span>

<span data-ttu-id="833a0-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="833a0-166">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="833a0-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="833a0-167">Response</span></span>

<span data-ttu-id="833a0-168">Im folgenden finden Sie ein Beispiel für die Antwort.</span><span class="sxs-lookup"><span data-stu-id="833a0-168">Here are example of the response.</span></span> 

<span data-ttu-id="833a0-169">Hinweis: die hier gezeigten Antwortobjekte können zur Kürze abgeschnitten werden.</span><span class="sxs-lookup"><span data-stu-id="833a0-169">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="833a0-170">Die für den Workflow geeigneten Eigenschaften werden zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="833a0-170">Properties appropriate for the workflow are returned.</span></span>

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



