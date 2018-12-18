---
title: Erstellen von „deviceComplianceUserStatus“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceUserStatus.
author: tfitzmac
ms.openlocfilehash: 417c6a2e87e274119fdbb480a7a2c8204dc81d3f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328175"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="89657-103">Erstellen von „deviceComplianceUserStatus“</span><span class="sxs-lookup"><span data-stu-id="89657-103">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="89657-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="89657-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89657-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="89657-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89657-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="89657-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89657-107">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="89657-107">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89657-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="89657-108">Prerequisites</span></span>
<span data-ttu-id="89657-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89657-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89657-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="89657-111">Permission type</span></span>|<span data-ttu-id="89657-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="89657-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89657-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="89657-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89657-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89657-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89657-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="89657-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89657-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89657-116">Not supported.</span></span>|
|<span data-ttu-id="89657-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="89657-117">Application</span></span>|<span data-ttu-id="89657-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89657-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89657-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="89657-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="89657-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="89657-120">Request headers</span></span>
|<span data-ttu-id="89657-121">Header</span><span class="sxs-lookup"><span data-stu-id="89657-121">Header</span></span>|<span data-ttu-id="89657-122">Wert</span><span class="sxs-lookup"><span data-stu-id="89657-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89657-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="89657-123">Authorization</span></span>|<span data-ttu-id="89657-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="89657-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89657-125">Accept</span><span class="sxs-lookup"><span data-stu-id="89657-125">Accept</span></span>|<span data-ttu-id="89657-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89657-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89657-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="89657-127">Request body</span></span>
<span data-ttu-id="89657-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceUserStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="89657-128">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="89657-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceUserStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="89657-129">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="89657-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="89657-130">Property</span></span>|<span data-ttu-id="89657-131">Typ</span><span class="sxs-lookup"><span data-stu-id="89657-131">Type</span></span>|<span data-ttu-id="89657-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89657-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89657-133">id</span><span class="sxs-lookup"><span data-stu-id="89657-133">id</span></span>|<span data-ttu-id="89657-134">String</span><span class="sxs-lookup"><span data-stu-id="89657-134">String</span></span>|<span data-ttu-id="89657-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="89657-135">Key of the entity.</span></span>|
|<span data-ttu-id="89657-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="89657-136">userDisplayName</span></span>|<span data-ttu-id="89657-137">String</span><span class="sxs-lookup"><span data-stu-id="89657-137">String</span></span>|<span data-ttu-id="89657-138">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="89657-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="89657-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="89657-139">devicesCount</span></span>|<span data-ttu-id="89657-140">Int32</span><span class="sxs-lookup"><span data-stu-id="89657-140">Int32</span></span>|<span data-ttu-id="89657-141">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="89657-141">Devices count for that user.</span></span>|
|<span data-ttu-id="89657-142">status</span><span class="sxs-lookup"><span data-stu-id="89657-142">status</span></span>|[<span data-ttu-id="89657-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="89657-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="89657-144">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="89657-144">Compliance status of the policy report.</span></span> <span data-ttu-id="89657-145">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="89657-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="89657-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="89657-146">lastReportedDateTime</span></span>|<span data-ttu-id="89657-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89657-147">DateTimeOffset</span></span>|<span data-ttu-id="89657-148">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="89657-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="89657-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="89657-149">userPrincipalName</span></span>|<span data-ttu-id="89657-150">String</span><span class="sxs-lookup"><span data-stu-id="89657-150">String</span></span>|<span data-ttu-id="89657-151">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="89657-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="89657-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="89657-152">Response</span></span>
<span data-ttu-id="89657-153">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="89657-153">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89657-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="89657-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="89657-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="89657-155">Request</span></span>
<span data-ttu-id="89657-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="89657-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="89657-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="89657-157">Response</span></span>
<span data-ttu-id="89657-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89657-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





