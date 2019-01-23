---
title: Aktualisieren von „deviceComplianceUserStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceComplianceUserStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0316f19ae718fbd358868fe7701d7ab833db75af
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416041"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="74986-103">Aktualisieren von „deviceComplianceUserStatus“</span><span class="sxs-lookup"><span data-stu-id="74986-103">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="74986-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="74986-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="74986-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="74986-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74986-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="74986-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74986-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="74986-107">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74986-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="74986-108">Prerequisites</span></span>
<span data-ttu-id="74986-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="74986-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="74986-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="74986-111">Permission type</span></span>|<span data-ttu-id="74986-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="74986-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74986-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="74986-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74986-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74986-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74986-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="74986-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74986-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74986-116">Not supported.</span></span>|
|<span data-ttu-id="74986-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="74986-117">Application</span></span>|<span data-ttu-id="74986-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74986-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74986-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="74986-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="74986-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="74986-120">Request headers</span></span>
|<span data-ttu-id="74986-121">Header</span><span class="sxs-lookup"><span data-stu-id="74986-121">Header</span></span>|<span data-ttu-id="74986-122">Wert</span><span class="sxs-lookup"><span data-stu-id="74986-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74986-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="74986-123">Authorization</span></span>|<span data-ttu-id="74986-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="74986-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74986-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="74986-125">Accept</span></span>|<span data-ttu-id="74986-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74986-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74986-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="74986-127">Request body</span></span>
<span data-ttu-id="74986-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="74986-128">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="74986-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="74986-129">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="74986-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="74986-130">Property</span></span>|<span data-ttu-id="74986-131">Typ</span><span class="sxs-lookup"><span data-stu-id="74986-131">Type</span></span>|<span data-ttu-id="74986-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74986-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74986-133">id</span><span class="sxs-lookup"><span data-stu-id="74986-133">id</span></span>|<span data-ttu-id="74986-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="74986-134">String</span></span>|<span data-ttu-id="74986-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="74986-135">Key of the entity.</span></span>|
|<span data-ttu-id="74986-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="74986-136">userDisplayName</span></span>|<span data-ttu-id="74986-137">String</span><span class="sxs-lookup"><span data-stu-id="74986-137">String</span></span>|<span data-ttu-id="74986-138">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="74986-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="74986-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="74986-139">devicesCount</span></span>|<span data-ttu-id="74986-140">Int32</span><span class="sxs-lookup"><span data-stu-id="74986-140">Int32</span></span>|<span data-ttu-id="74986-141">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="74986-141">Devices count for that user.</span></span>|
|<span data-ttu-id="74986-142">status</span><span class="sxs-lookup"><span data-stu-id="74986-142">status</span></span>|[<span data-ttu-id="74986-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="74986-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="74986-144">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="74986-144">Compliance status of the policy report.</span></span> <span data-ttu-id="74986-145">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="74986-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="74986-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="74986-146">lastReportedDateTime</span></span>|<span data-ttu-id="74986-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74986-147">DateTimeOffset</span></span>|<span data-ttu-id="74986-148">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="74986-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="74986-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="74986-149">userPrincipalName</span></span>|<span data-ttu-id="74986-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="74986-150">String</span></span>|<span data-ttu-id="74986-151">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="74986-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="74986-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="74986-152">Response</span></span>
<span data-ttu-id="74986-153">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="74986-153">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74986-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="74986-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="74986-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74986-155">Request</span></span>
<span data-ttu-id="74986-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="74986-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
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

### <a name="response"></a><span data-ttu-id="74986-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="74986-157">Response</span></span>
<span data-ttu-id="74986-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74986-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




