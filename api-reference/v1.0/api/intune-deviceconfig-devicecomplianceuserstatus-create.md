---
title: Erstellen von „deviceComplianceUserStatus“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceUserStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b4e82a3ead9e4ab36fd5f94a71afc5558f7482de
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849322"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="050e4-103">Erstellen von „deviceComplianceUserStatus“</span><span class="sxs-lookup"><span data-stu-id="050e4-103">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="050e4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="050e4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="050e4-105">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="050e4-105">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="050e4-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="050e4-106">Prerequisites</span></span>
<span data-ttu-id="050e4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="050e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="050e4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="050e4-109">Permission type</span></span>|<span data-ttu-id="050e4-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="050e4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="050e4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="050e4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="050e4-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="050e4-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="050e4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="050e4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="050e4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="050e4-114">Not supported.</span></span>|
|<span data-ttu-id="050e4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="050e4-115">Application</span></span>|<span data-ttu-id="050e4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="050e4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="050e4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="050e4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="050e4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="050e4-118">Request headers</span></span>
|<span data-ttu-id="050e4-119">Header</span><span class="sxs-lookup"><span data-stu-id="050e4-119">Header</span></span>|<span data-ttu-id="050e4-120">Wert</span><span class="sxs-lookup"><span data-stu-id="050e4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="050e4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="050e4-121">Authorization</span></span>|<span data-ttu-id="050e4-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="050e4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="050e4-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="050e4-123">Accept</span></span>|<span data-ttu-id="050e4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="050e4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="050e4-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="050e4-125">Request body</span></span>
<span data-ttu-id="050e4-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceUserStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="050e4-126">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="050e4-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceUserStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="050e4-127">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="050e4-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="050e4-128">Property</span></span>|<span data-ttu-id="050e4-129">Typ</span><span class="sxs-lookup"><span data-stu-id="050e4-129">Type</span></span>|<span data-ttu-id="050e4-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="050e4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="050e4-131">id</span><span class="sxs-lookup"><span data-stu-id="050e4-131">id</span></span>|<span data-ttu-id="050e4-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="050e4-132">String</span></span>|<span data-ttu-id="050e4-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="050e4-133">Key of the entity.</span></span>|
|<span data-ttu-id="050e4-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="050e4-134">userDisplayName</span></span>|<span data-ttu-id="050e4-135">String</span><span class="sxs-lookup"><span data-stu-id="050e4-135">String</span></span>|<span data-ttu-id="050e4-136">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="050e4-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="050e4-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="050e4-137">devicesCount</span></span>|<span data-ttu-id="050e4-138">Int32</span><span class="sxs-lookup"><span data-stu-id="050e4-138">Int32</span></span>|<span data-ttu-id="050e4-139">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="050e4-139">Devices count for that user.</span></span>|
|<span data-ttu-id="050e4-140">status</span><span class="sxs-lookup"><span data-stu-id="050e4-140">status</span></span>|[<span data-ttu-id="050e4-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="050e4-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="050e4-142">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="050e4-142">Compliance status of the policy report.</span></span> <span data-ttu-id="050e4-143">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="050e4-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="050e4-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="050e4-144">lastReportedDateTime</span></span>|<span data-ttu-id="050e4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="050e4-145">DateTimeOffset</span></span>|<span data-ttu-id="050e4-146">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="050e4-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="050e4-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="050e4-147">userPrincipalName</span></span>|<span data-ttu-id="050e4-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="050e4-148">String</span></span>|<span data-ttu-id="050e4-149">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="050e4-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="050e4-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="050e4-150">Response</span></span>
<span data-ttu-id="050e4-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="050e4-151">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="050e4-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="050e4-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="050e4-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="050e4-153">Request</span></span>
<span data-ttu-id="050e4-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="050e4-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="050e4-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="050e4-155">Response</span></span>
<span data-ttu-id="050e4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="050e4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



