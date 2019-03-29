---
title: Erstellen von „deviceComplianceUserStatus“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b5b3d3586cd1c50f0a3372dfe06d75f817341cb4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960923"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="d7da4-103">Erstellen von „deviceComplianceUserStatus“</span><span class="sxs-lookup"><span data-stu-id="d7da4-103">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="d7da4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d7da4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7da4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d7da4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7da4-106">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="d7da4-106">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7da4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d7da4-107">Prerequisites</span></span>
<span data-ttu-id="d7da4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7da4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7da4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d7da4-110">Permission type</span></span>|<span data-ttu-id="d7da4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d7da4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7da4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d7da4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7da4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7da4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7da4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d7da4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7da4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7da4-115">Not supported.</span></span>|
|<span data-ttu-id="d7da4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d7da4-116">Application</span></span>|<span data-ttu-id="d7da4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7da4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7da4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7da4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="d7da4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d7da4-119">Request headers</span></span>
|<span data-ttu-id="d7da4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d7da4-120">Header</span></span>|<span data-ttu-id="d7da4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d7da4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7da4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7da4-122">Authorization</span></span>|<span data-ttu-id="d7da4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d7da4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7da4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d7da4-124">Accept</span></span>|<span data-ttu-id="d7da4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7da4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7da4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d7da4-126">Request body</span></span>
<span data-ttu-id="d7da4-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceUserStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="d7da4-127">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="d7da4-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceUserStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="d7da4-128">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="d7da4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d7da4-129">Property</span></span>|<span data-ttu-id="d7da4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d7da4-130">Type</span></span>|<span data-ttu-id="d7da4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7da4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7da4-132">id</span><span class="sxs-lookup"><span data-stu-id="d7da4-132">id</span></span>|<span data-ttu-id="d7da4-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d7da4-133">String</span></span>|<span data-ttu-id="d7da4-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d7da4-134">Key of the entity.</span></span>|
|<span data-ttu-id="d7da4-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d7da4-135">userDisplayName</span></span>|<span data-ttu-id="d7da4-136">String</span><span class="sxs-lookup"><span data-stu-id="d7da4-136">String</span></span>|<span data-ttu-id="d7da4-137">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="d7da4-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="d7da4-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="d7da4-138">devicesCount</span></span>|<span data-ttu-id="d7da4-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d7da4-139">Int32</span></span>|<span data-ttu-id="d7da4-140">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="d7da4-140">Devices count for that user.</span></span>|
|<span data-ttu-id="d7da4-141">status</span><span class="sxs-lookup"><span data-stu-id="d7da4-141">status</span></span>|[<span data-ttu-id="d7da4-142">Wurde</span><span class="sxs-lookup"><span data-stu-id="d7da4-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d7da4-143">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="d7da4-143">Compliance status of the policy report.</span></span> <span data-ttu-id="d7da4-144">Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="d7da4-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d7da4-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7da4-145">lastReportedDateTime</span></span>|<span data-ttu-id="d7da4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7da4-146">DateTimeOffset</span></span>|<span data-ttu-id="d7da4-147">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="d7da4-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="d7da4-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d7da4-148">userPrincipalName</span></span>|<span data-ttu-id="d7da4-149">String</span><span class="sxs-lookup"><span data-stu-id="d7da4-149">String</span></span>|<span data-ttu-id="d7da4-150">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="d7da4-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="d7da4-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7da4-151">Response</span></span>
<span data-ttu-id="d7da4-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d7da4-152">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7da4-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d7da4-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7da4-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7da4-154">Request</span></span>
<span data-ttu-id="d7da4-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d7da4-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d7da4-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7da4-156">Response</span></span>
<span data-ttu-id="d7da4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7da4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




