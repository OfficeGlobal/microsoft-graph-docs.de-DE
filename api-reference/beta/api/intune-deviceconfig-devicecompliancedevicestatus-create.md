---
title: Erstellen von „deviceComplianceDeviceStatus“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2ad91ad1e7ccd75821ae64440e88344f7f8b9c3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948338"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="82359-103">Erstellen von „deviceComplianceDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="82359-103">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="82359-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="82359-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82359-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="82359-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82359-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="82359-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82359-107">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="82359-107">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82359-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="82359-108">Prerequisites</span></span>
<span data-ttu-id="82359-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82359-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82359-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="82359-111">Permission type</span></span>|<span data-ttu-id="82359-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="82359-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82359-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="82359-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82359-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82359-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82359-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="82359-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82359-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="82359-116">Not supported.</span></span>|
|<span data-ttu-id="82359-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="82359-117">Application</span></span>|<span data-ttu-id="82359-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="82359-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82359-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="82359-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="82359-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="82359-120">Request headers</span></span>
|<span data-ttu-id="82359-121">Header</span><span class="sxs-lookup"><span data-stu-id="82359-121">Header</span></span>|<span data-ttu-id="82359-122">Wert</span><span class="sxs-lookup"><span data-stu-id="82359-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82359-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="82359-123">Authorization</span></span>|<span data-ttu-id="82359-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="82359-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82359-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="82359-125">Accept</span></span>|<span data-ttu-id="82359-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82359-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82359-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="82359-127">Request body</span></span>
<span data-ttu-id="82359-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="82359-128">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="82359-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="82359-129">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="82359-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="82359-130">Property</span></span>|<span data-ttu-id="82359-131">Typ</span><span class="sxs-lookup"><span data-stu-id="82359-131">Type</span></span>|<span data-ttu-id="82359-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82359-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82359-133">id</span><span class="sxs-lookup"><span data-stu-id="82359-133">id</span></span>|<span data-ttu-id="82359-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="82359-134">String</span></span>|<span data-ttu-id="82359-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="82359-135">Key of the entity.</span></span>|
|<span data-ttu-id="82359-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="82359-136">deviceDisplayName</span></span>|<span data-ttu-id="82359-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="82359-137">String</span></span>|<span data-ttu-id="82359-138">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="82359-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="82359-139">userName</span><span class="sxs-lookup"><span data-stu-id="82359-139">userName</span></span>|<span data-ttu-id="82359-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="82359-140">String</span></span>|<span data-ttu-id="82359-141">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="82359-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="82359-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="82359-142">deviceModel</span></span>|<span data-ttu-id="82359-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="82359-143">String</span></span>|<span data-ttu-id="82359-144">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="82359-144">The device model that is being reported</span></span>|
|<span data-ttu-id="82359-145">Plattform</span><span class="sxs-lookup"><span data-stu-id="82359-145">platform</span></span>|<span data-ttu-id="82359-146">Int32</span><span class="sxs-lookup"><span data-stu-id="82359-146">Int32</span></span>|<span data-ttu-id="82359-147">Plattform des Geräts, das gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="82359-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="82359-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="82359-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="82359-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82359-149">DateTimeOffset</span></span>|<span data-ttu-id="82359-150">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="82359-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="82359-151">status</span><span class="sxs-lookup"><span data-stu-id="82359-151">status</span></span>|[<span data-ttu-id="82359-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="82359-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="82359-153">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="82359-153">Compliance status of the policy report.</span></span> <span data-ttu-id="82359-154">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="82359-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="82359-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="82359-155">lastReportedDateTime</span></span>|<span data-ttu-id="82359-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82359-156">DateTimeOffset</span></span>|<span data-ttu-id="82359-157">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="82359-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="82359-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="82359-158">userPrincipalName</span></span>|<span data-ttu-id="82359-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="82359-159">String</span></span>|<span data-ttu-id="82359-160">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="82359-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="82359-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="82359-161">Response</span></span>
<span data-ttu-id="82359-162">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="82359-162">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82359-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="82359-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="82359-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="82359-164">Request</span></span>
<span data-ttu-id="82359-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="82359-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82359-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="82359-166">Response</span></span>
<span data-ttu-id="82359-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="82359-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





