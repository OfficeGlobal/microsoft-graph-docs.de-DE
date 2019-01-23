---
title: Erstellen von „deviceComplianceDeviceStatus“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0b9e7a7049c656c42f2ad843bedafcc6f9975619
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417574"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="5d8d9-103">Erstellen von „deviceComplianceDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="5d8d9-103">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="5d8d9-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5d8d9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5d8d9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5d8d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d8d9-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5d8d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d8d9-107">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="5d8d9-107">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d8d9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5d8d9-108">Prerequisites</span></span>
<span data-ttu-id="5d8d9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d8d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5d8d9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d8d9-111">Permission type</span></span>|<span data-ttu-id="5d8d9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d8d9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d8d9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d8d9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d8d9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d8d9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5d8d9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d8d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d8d9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d8d9-116">Not supported.</span></span>|
|<span data-ttu-id="5d8d9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d8d9-117">Application</span></span>|<span data-ttu-id="5d8d9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d8d9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d8d9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d8d9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="5d8d9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d8d9-120">Request headers</span></span>
|<span data-ttu-id="5d8d9-121">Header</span><span class="sxs-lookup"><span data-stu-id="5d8d9-121">Header</span></span>|<span data-ttu-id="5d8d9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5d8d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d8d9-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5d8d9-123">Authorization</span></span>|<span data-ttu-id="5d8d9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5d8d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d8d9-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5d8d9-125">Accept</span></span>|<span data-ttu-id="5d8d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d8d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d8d9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5d8d9-127">Request body</span></span>
<span data-ttu-id="5d8d9-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="5d8d9-128">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="5d8d9-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="5d8d9-129">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="5d8d9-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5d8d9-130">Property</span></span>|<span data-ttu-id="5d8d9-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5d8d9-131">Type</span></span>|<span data-ttu-id="5d8d9-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d8d9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d8d9-133">id</span><span class="sxs-lookup"><span data-stu-id="5d8d9-133">id</span></span>|<span data-ttu-id="5d8d9-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5d8d9-134">String</span></span>|<span data-ttu-id="5d8d9-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5d8d9-135">Key of the entity.</span></span>|
|<span data-ttu-id="5d8d9-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="5d8d9-136">deviceDisplayName</span></span>|<span data-ttu-id="5d8d9-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5d8d9-137">String</span></span>|<span data-ttu-id="5d8d9-138">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="5d8d9-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="5d8d9-139">userName</span><span class="sxs-lookup"><span data-stu-id="5d8d9-139">userName</span></span>|<span data-ttu-id="5d8d9-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5d8d9-140">String</span></span>|<span data-ttu-id="5d8d9-141">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="5d8d9-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="5d8d9-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="5d8d9-142">deviceModel</span></span>|<span data-ttu-id="5d8d9-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5d8d9-143">String</span></span>|<span data-ttu-id="5d8d9-144">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="5d8d9-144">The device model that is being reported</span></span>|
|<span data-ttu-id="5d8d9-145">Plattform</span><span class="sxs-lookup"><span data-stu-id="5d8d9-145">platform</span></span>|<span data-ttu-id="5d8d9-146">Int32</span><span class="sxs-lookup"><span data-stu-id="5d8d9-146">Int32</span></span>|<span data-ttu-id="5d8d9-147">Plattform des Geräts, das gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="5d8d9-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="5d8d9-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5d8d9-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="5d8d9-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d8d9-149">DateTimeOffset</span></span>|<span data-ttu-id="5d8d9-150">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="5d8d9-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="5d8d9-151">status</span><span class="sxs-lookup"><span data-stu-id="5d8d9-151">status</span></span>|[<span data-ttu-id="5d8d9-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="5d8d9-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5d8d9-153">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="5d8d9-153">Compliance status of the policy report.</span></span> <span data-ttu-id="5d8d9-154">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="5d8d9-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5d8d9-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d8d9-155">lastReportedDateTime</span></span>|<span data-ttu-id="5d8d9-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d8d9-156">DateTimeOffset</span></span>|<span data-ttu-id="5d8d9-157">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="5d8d9-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="5d8d9-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5d8d9-158">userPrincipalName</span></span>|<span data-ttu-id="5d8d9-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5d8d9-159">String</span></span>|<span data-ttu-id="5d8d9-160">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="5d8d9-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="5d8d9-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d8d9-161">Response</span></span>
<span data-ttu-id="5d8d9-162">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5d8d9-162">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d8d9-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d8d9-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d8d9-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d8d9-164">Request</span></span>
<span data-ttu-id="5d8d9-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d8d9-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5d8d9-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d8d9-166">Response</span></span>
<span data-ttu-id="5d8d9-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d8d9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




