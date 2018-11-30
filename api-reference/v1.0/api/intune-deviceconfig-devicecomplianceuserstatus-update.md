---
title: Aktualisieren von „deviceComplianceUserStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceComplianceUserStatus.
ms.openlocfilehash: a3994c12cc4e28b034746b8af21ece4f63eb85dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017385"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="8d2bb-103">Aktualisieren von „deviceComplianceUserStatus“</span><span class="sxs-lookup"><span data-stu-id="8d2bb-103">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="8d2bb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8d2bb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d2bb-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="8d2bb-105">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d2bb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8d2bb-106">Prerequisites</span></span>
<span data-ttu-id="8d2bb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d2bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d2bb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d2bb-109">Permission type</span></span>|<span data-ttu-id="8d2bb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d2bb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d2bb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d2bb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8d2bb-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d2bb-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d2bb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d2bb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d2bb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d2bb-114">Not supported.</span></span>|
|<span data-ttu-id="8d2bb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d2bb-115">Application</span></span>|<span data-ttu-id="8d2bb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d2bb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d2bb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d2bb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="8d2bb-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d2bb-118">Request headers</span></span>
|<span data-ttu-id="8d2bb-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8d2bb-119">Header</span></span>|<span data-ttu-id="8d2bb-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8d2bb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d2bb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d2bb-121">Authorization</span></span>|<span data-ttu-id="8d2bb-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8d2bb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d2bb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8d2bb-123">Accept</span></span>|<span data-ttu-id="8d2bb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8d2bb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d2bb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d2bb-125">Request body</span></span>
<span data-ttu-id="8d2bb-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="8d2bb-126">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="8d2bb-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="8d2bb-127">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="8d2bb-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8d2bb-128">Property</span></span>|<span data-ttu-id="8d2bb-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8d2bb-129">Type</span></span>|<span data-ttu-id="8d2bb-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d2bb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d2bb-131">id</span><span class="sxs-lookup"><span data-stu-id="8d2bb-131">id</span></span>|<span data-ttu-id="8d2bb-132">String</span><span class="sxs-lookup"><span data-stu-id="8d2bb-132">String</span></span>|<span data-ttu-id="8d2bb-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8d2bb-133">Key of the entity.</span></span>|
|<span data-ttu-id="8d2bb-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8d2bb-134">userDisplayName</span></span>|<span data-ttu-id="8d2bb-135">String</span><span class="sxs-lookup"><span data-stu-id="8d2bb-135">String</span></span>|<span data-ttu-id="8d2bb-136">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="8d2bb-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="8d2bb-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="8d2bb-137">devicesCount</span></span>|<span data-ttu-id="8d2bb-138">Int32</span><span class="sxs-lookup"><span data-stu-id="8d2bb-138">Int32</span></span>|<span data-ttu-id="8d2bb-139">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="8d2bb-139">Devices count for that user.</span></span>|
|<span data-ttu-id="8d2bb-140">status</span><span class="sxs-lookup"><span data-stu-id="8d2bb-140">status</span></span>|[<span data-ttu-id="8d2bb-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="8d2bb-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8d2bb-142">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="8d2bb-142">Compliance status of the policy report.</span></span> <span data-ttu-id="8d2bb-143">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="8d2bb-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8d2bb-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d2bb-144">lastReportedDateTime</span></span>|<span data-ttu-id="8d2bb-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d2bb-145">DateTimeOffset</span></span>|<span data-ttu-id="8d2bb-146">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="8d2bb-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="8d2bb-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8d2bb-147">userPrincipalName</span></span>|<span data-ttu-id="8d2bb-148">String</span><span class="sxs-lookup"><span data-stu-id="8d2bb-148">String</span></span>|<span data-ttu-id="8d2bb-149">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="8d2bb-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="8d2bb-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d2bb-150">Response</span></span>
<span data-ttu-id="8d2bb-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8d2bb-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d2bb-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d2bb-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d2bb-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d2bb-153">Request</span></span>
<span data-ttu-id="8d2bb-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d2bb-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
Content-type: application/json
Content-length: 287

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="8d2bb-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d2bb-155">Response</span></span>
<span data-ttu-id="8d2bb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d2bb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 336

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



