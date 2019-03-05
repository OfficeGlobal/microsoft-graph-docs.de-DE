---
title: Erstellen von „deviceComplianceUserStatus“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd489d69656408d840684c5b1f1f7c17f238cd4e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141860"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="ff678-103">Erstellen von „deviceComplianceUserStatus“</span><span class="sxs-lookup"><span data-stu-id="ff678-103">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="ff678-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff678-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff678-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ff678-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff678-106">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="ff678-106">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff678-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ff678-107">Prerequisites</span></span>
<span data-ttu-id="ff678-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ff678-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ff678-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff678-110">Permission type</span></span>|<span data-ttu-id="ff678-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff678-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff678-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff678-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff678-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff678-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff678-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff678-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff678-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff678-115">Not supported.</span></span>|
|<span data-ttu-id="ff678-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff678-116">Application</span></span>|<span data-ttu-id="ff678-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff678-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff678-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff678-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ff678-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff678-119">Request headers</span></span>
|<span data-ttu-id="ff678-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ff678-120">Header</span></span>|<span data-ttu-id="ff678-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ff678-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff678-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff678-122">Authorization</span></span>|<span data-ttu-id="ff678-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ff678-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff678-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ff678-124">Accept</span></span>|<span data-ttu-id="ff678-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff678-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff678-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff678-126">Request body</span></span>
<span data-ttu-id="ff678-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceUserStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="ff678-127">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="ff678-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceUserStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="ff678-128">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="ff678-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff678-129">Property</span></span>|<span data-ttu-id="ff678-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ff678-130">Type</span></span>|<span data-ttu-id="ff678-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff678-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff678-132">id</span><span class="sxs-lookup"><span data-stu-id="ff678-132">id</span></span>|<span data-ttu-id="ff678-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff678-133">String</span></span>|<span data-ttu-id="ff678-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ff678-134">Key of the entity.</span></span>|
|<span data-ttu-id="ff678-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ff678-135">userDisplayName</span></span>|<span data-ttu-id="ff678-136">String</span><span class="sxs-lookup"><span data-stu-id="ff678-136">String</span></span>|<span data-ttu-id="ff678-137">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="ff678-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ff678-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="ff678-138">devicesCount</span></span>|<span data-ttu-id="ff678-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ff678-139">Int32</span></span>|<span data-ttu-id="ff678-140">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="ff678-140">Devices count for that user.</span></span>|
|<span data-ttu-id="ff678-141">status</span><span class="sxs-lookup"><span data-stu-id="ff678-141">status</span></span>|[<span data-ttu-id="ff678-142">Wurde</span><span class="sxs-lookup"><span data-stu-id="ff678-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ff678-143">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="ff678-143">Compliance status of the policy report.</span></span> <span data-ttu-id="ff678-144">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="ff678-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ff678-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff678-145">lastReportedDateTime</span></span>|<span data-ttu-id="ff678-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff678-146">DateTimeOffset</span></span>|<span data-ttu-id="ff678-147">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="ff678-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ff678-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ff678-148">userPrincipalName</span></span>|<span data-ttu-id="ff678-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff678-149">String</span></span>|<span data-ttu-id="ff678-150">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="ff678-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="ff678-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff678-151">Response</span></span>
<span data-ttu-id="ff678-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ff678-152">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff678-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ff678-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff678-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff678-154">Request</span></span>
<span data-ttu-id="ff678-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ff678-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="ff678-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff678-156">Response</span></span>
<span data-ttu-id="ff678-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff678-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




