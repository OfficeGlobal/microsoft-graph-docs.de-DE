---
title: Erstellen von „deviceComplianceDeviceStatus“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 13e7d217ce35baca2fb2742968b2b35b79ca7473
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817143"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="43849-103">Erstellen von „deviceComplianceDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="43849-103">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="43849-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="43849-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43849-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="43849-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43849-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="43849-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43849-107">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="43849-107">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43849-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="43849-108">Prerequisites</span></span>
<span data-ttu-id="43849-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43849-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43849-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="43849-111">Permission type</span></span>|<span data-ttu-id="43849-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="43849-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43849-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="43849-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43849-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43849-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43849-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="43849-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43849-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43849-116">Not supported.</span></span>|
|<span data-ttu-id="43849-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="43849-117">Application</span></span>|<span data-ttu-id="43849-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43849-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43849-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="43849-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="43849-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="43849-120">Request headers</span></span>
|<span data-ttu-id="43849-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="43849-121">Header</span></span>|<span data-ttu-id="43849-122">Wert</span><span class="sxs-lookup"><span data-stu-id="43849-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43849-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43849-123">Authorization</span></span>|<span data-ttu-id="43849-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="43849-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43849-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="43849-125">Accept</span></span>|<span data-ttu-id="43849-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43849-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43849-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="43849-127">Request body</span></span>
<span data-ttu-id="43849-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="43849-128">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="43849-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="43849-129">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="43849-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="43849-130">Property</span></span>|<span data-ttu-id="43849-131">Typ</span><span class="sxs-lookup"><span data-stu-id="43849-131">Type</span></span>|<span data-ttu-id="43849-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43849-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43849-133">id</span><span class="sxs-lookup"><span data-stu-id="43849-133">id</span></span>|<span data-ttu-id="43849-134">String</span><span class="sxs-lookup"><span data-stu-id="43849-134">String</span></span>|<span data-ttu-id="43849-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="43849-135">Key of the entity.</span></span>|
|<span data-ttu-id="43849-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="43849-136">deviceDisplayName</span></span>|<span data-ttu-id="43849-137">String</span><span class="sxs-lookup"><span data-stu-id="43849-137">String</span></span>|<span data-ttu-id="43849-138">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="43849-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="43849-139">userName</span><span class="sxs-lookup"><span data-stu-id="43849-139">userName</span></span>|<span data-ttu-id="43849-140">String</span><span class="sxs-lookup"><span data-stu-id="43849-140">String</span></span>|<span data-ttu-id="43849-141">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="43849-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="43849-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="43849-142">deviceModel</span></span>|<span data-ttu-id="43849-143">String</span><span class="sxs-lookup"><span data-stu-id="43849-143">String</span></span>|<span data-ttu-id="43849-144">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="43849-144">The device model that is being reported</span></span>|
|<span data-ttu-id="43849-145">Plattform</span><span class="sxs-lookup"><span data-stu-id="43849-145">platform</span></span>|<span data-ttu-id="43849-146">Int32</span><span class="sxs-lookup"><span data-stu-id="43849-146">Int32</span></span>|<span data-ttu-id="43849-147">Plattform des Geräts, das gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="43849-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="43849-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="43849-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="43849-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43849-149">DateTimeOffset</span></span>|<span data-ttu-id="43849-150">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="43849-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="43849-151">status</span><span class="sxs-lookup"><span data-stu-id="43849-151">status</span></span>|[<span data-ttu-id="43849-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="43849-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="43849-153">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="43849-153">Compliance status of the policy report.</span></span> <span data-ttu-id="43849-154">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="43849-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="43849-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="43849-155">lastReportedDateTime</span></span>|<span data-ttu-id="43849-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43849-156">DateTimeOffset</span></span>|<span data-ttu-id="43849-157">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="43849-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="43849-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="43849-158">userPrincipalName</span></span>|<span data-ttu-id="43849-159">String</span><span class="sxs-lookup"><span data-stu-id="43849-159">String</span></span>|<span data-ttu-id="43849-160">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="43849-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="43849-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="43849-161">Response</span></span>
<span data-ttu-id="43849-162">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="43849-162">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43849-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="43849-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="43849-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="43849-164">Request</span></span>
<span data-ttu-id="43849-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="43849-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
Content-type: application/json
Content-length: 444

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="43849-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="43849-166">Response</span></span>
<span data-ttu-id="43849-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43849-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 493

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```





