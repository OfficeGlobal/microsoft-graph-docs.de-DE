---
title: Aktualisieren von „deviceComplianceDeviceStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceComplianceDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 35273f196231912f8343130e5a58ff62949579ac
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425491"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="49191-103">Aktualisieren von „deviceComplianceDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="49191-103">Update deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="49191-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="49191-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="49191-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="49191-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49191-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="49191-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49191-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="49191-107">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49191-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="49191-108">Prerequisites</span></span>
<span data-ttu-id="49191-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="49191-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="49191-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="49191-111">Permission type</span></span>|<span data-ttu-id="49191-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="49191-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49191-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="49191-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49191-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49191-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49191-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="49191-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49191-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49191-116">Not supported.</span></span>|
|<span data-ttu-id="49191-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="49191-117">Application</span></span>|<span data-ttu-id="49191-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49191-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49191-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="49191-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="49191-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="49191-120">Request headers</span></span>
|<span data-ttu-id="49191-121">Header</span><span class="sxs-lookup"><span data-stu-id="49191-121">Header</span></span>|<span data-ttu-id="49191-122">Wert</span><span class="sxs-lookup"><span data-stu-id="49191-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49191-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="49191-123">Authorization</span></span>|<span data-ttu-id="49191-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="49191-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49191-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="49191-125">Accept</span></span>|<span data-ttu-id="49191-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49191-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49191-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="49191-127">Request body</span></span>
<span data-ttu-id="49191-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="49191-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="49191-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="49191-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="49191-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="49191-130">Property</span></span>|<span data-ttu-id="49191-131">Typ</span><span class="sxs-lookup"><span data-stu-id="49191-131">Type</span></span>|<span data-ttu-id="49191-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49191-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49191-133">id</span><span class="sxs-lookup"><span data-stu-id="49191-133">id</span></span>|<span data-ttu-id="49191-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49191-134">String</span></span>|<span data-ttu-id="49191-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="49191-135">Key of the entity.</span></span>|
|<span data-ttu-id="49191-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="49191-136">deviceDisplayName</span></span>|<span data-ttu-id="49191-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49191-137">String</span></span>|<span data-ttu-id="49191-138">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="49191-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="49191-139">userName</span><span class="sxs-lookup"><span data-stu-id="49191-139">userName</span></span>|<span data-ttu-id="49191-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49191-140">String</span></span>|<span data-ttu-id="49191-141">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="49191-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="49191-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="49191-142">deviceModel</span></span>|<span data-ttu-id="49191-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49191-143">String</span></span>|<span data-ttu-id="49191-144">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="49191-144">The device model that is being reported</span></span>|
|<span data-ttu-id="49191-145">Plattform</span><span class="sxs-lookup"><span data-stu-id="49191-145">platform</span></span>|<span data-ttu-id="49191-146">Int32</span><span class="sxs-lookup"><span data-stu-id="49191-146">Int32</span></span>|<span data-ttu-id="49191-147">Plattform des Geräts, das gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="49191-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="49191-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="49191-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="49191-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49191-149">DateTimeOffset</span></span>|<span data-ttu-id="49191-150">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="49191-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="49191-151">status</span><span class="sxs-lookup"><span data-stu-id="49191-151">status</span></span>|[<span data-ttu-id="49191-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="49191-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="49191-153">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="49191-153">Compliance status of the policy report.</span></span> <span data-ttu-id="49191-154">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="49191-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="49191-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="49191-155">lastReportedDateTime</span></span>|<span data-ttu-id="49191-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49191-156">DateTimeOffset</span></span>|<span data-ttu-id="49191-157">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="49191-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="49191-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="49191-158">userPrincipalName</span></span>|<span data-ttu-id="49191-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49191-159">String</span></span>|<span data-ttu-id="49191-160">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="49191-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="49191-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="49191-161">Response</span></span>
<span data-ttu-id="49191-162">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="49191-162">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49191-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="49191-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="49191-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="49191-164">Request</span></span>
<span data-ttu-id="49191-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="49191-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
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

### <a name="response"></a><span data-ttu-id="49191-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="49191-166">Response</span></span>
<span data-ttu-id="49191-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49191-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




