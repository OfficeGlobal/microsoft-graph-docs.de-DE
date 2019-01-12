---
title: Erstellen von „deviceComplianceDeviceStatus“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9e75a0a89ff16bafdf3f4b4fc6cd4cb9fbd0260b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952419"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="bdd66-103">Erstellen von „deviceComplianceDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="bdd66-103">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="bdd66-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bdd66-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdd66-105">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="bdd66-105">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bdd66-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bdd66-106">Prerequisites</span></span>
<span data-ttu-id="bdd66-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdd66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdd66-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bdd66-109">Permission type</span></span>|<span data-ttu-id="bdd66-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bdd66-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdd66-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bdd66-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bdd66-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdd66-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bdd66-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bdd66-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdd66-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bdd66-114">Not supported.</span></span>|
|<span data-ttu-id="bdd66-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bdd66-115">Application</span></span>|<span data-ttu-id="bdd66-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bdd66-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdd66-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bdd66-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="bdd66-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bdd66-118">Request headers</span></span>
|<span data-ttu-id="bdd66-119">Header</span><span class="sxs-lookup"><span data-stu-id="bdd66-119">Header</span></span>|<span data-ttu-id="bdd66-120">Wert</span><span class="sxs-lookup"><span data-stu-id="bdd66-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdd66-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdd66-121">Authorization</span></span>|<span data-ttu-id="bdd66-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bdd66-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdd66-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bdd66-123">Accept</span></span>|<span data-ttu-id="bdd66-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bdd66-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdd66-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bdd66-125">Request body</span></span>
<span data-ttu-id="bdd66-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="bdd66-126">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="bdd66-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="bdd66-127">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="bdd66-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bdd66-128">Property</span></span>|<span data-ttu-id="bdd66-129">Typ</span><span class="sxs-lookup"><span data-stu-id="bdd66-129">Type</span></span>|<span data-ttu-id="bdd66-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bdd66-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdd66-131">id</span><span class="sxs-lookup"><span data-stu-id="bdd66-131">id</span></span>|<span data-ttu-id="bdd66-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bdd66-132">String</span></span>|<span data-ttu-id="bdd66-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bdd66-133">Key of the entity.</span></span>|
|<span data-ttu-id="bdd66-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="bdd66-134">deviceDisplayName</span></span>|<span data-ttu-id="bdd66-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bdd66-135">String</span></span>|<span data-ttu-id="bdd66-136">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="bdd66-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="bdd66-137">userName</span><span class="sxs-lookup"><span data-stu-id="bdd66-137">userName</span></span>|<span data-ttu-id="bdd66-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bdd66-138">String</span></span>|<span data-ttu-id="bdd66-139">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="bdd66-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="bdd66-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="bdd66-140">deviceModel</span></span>|<span data-ttu-id="bdd66-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bdd66-141">String</span></span>|<span data-ttu-id="bdd66-142">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="bdd66-142">The device model that is being reported</span></span>|
|<span data-ttu-id="bdd66-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bdd66-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="bdd66-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdd66-144">DateTimeOffset</span></span>|<span data-ttu-id="bdd66-145">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="bdd66-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="bdd66-146">status</span><span class="sxs-lookup"><span data-stu-id="bdd66-146">status</span></span>|[<span data-ttu-id="bdd66-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="bdd66-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="bdd66-148">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="bdd66-148">Compliance status of the policy report.</span></span> <span data-ttu-id="bdd66-149">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="bdd66-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="bdd66-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="bdd66-150">lastReportedDateTime</span></span>|<span data-ttu-id="bdd66-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdd66-151">DateTimeOffset</span></span>|<span data-ttu-id="bdd66-152">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="bdd66-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="bdd66-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bdd66-153">userPrincipalName</span></span>|<span data-ttu-id="bdd66-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bdd66-154">String</span></span>|<span data-ttu-id="bdd66-155">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="bdd66-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="bdd66-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="bdd66-156">Response</span></span>
<span data-ttu-id="bdd66-157">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bdd66-157">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdd66-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bdd66-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="bdd66-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bdd66-159">Request</span></span>
<span data-ttu-id="bdd66-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bdd66-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
Content-type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="bdd66-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="bdd66-161">Response</span></span>
<span data-ttu-id="bdd66-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bdd66-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



