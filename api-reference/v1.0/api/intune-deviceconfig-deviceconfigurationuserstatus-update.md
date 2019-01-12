---
title: Aktualisieren von „deviceConfigurationUserStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a4f54f3e5280e6b0cdf5526e8eccc0bc7ee7b7ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972047"
---
# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="2972d-103">Aktualisieren von „deviceConfigurationUserStatus“</span><span class="sxs-lookup"><span data-stu-id="2972d-103">Update deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="2972d-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2972d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2972d-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="2972d-105">Update the properties of a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2972d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2972d-106">Prerequisites</span></span>
<span data-ttu-id="2972d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2972d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2972d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2972d-109">Permission type</span></span>|<span data-ttu-id="2972d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2972d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2972d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2972d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2972d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2972d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2972d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2972d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2972d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2972d-114">Not supported.</span></span>|
|<span data-ttu-id="2972d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2972d-115">Application</span></span>|<span data-ttu-id="2972d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2972d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2972d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2972d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="2972d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2972d-118">Request headers</span></span>
|<span data-ttu-id="2972d-119">Header</span><span class="sxs-lookup"><span data-stu-id="2972d-119">Header</span></span>|<span data-ttu-id="2972d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2972d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2972d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2972d-121">Authorization</span></span>|<span data-ttu-id="2972d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2972d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2972d-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2972d-123">Accept</span></span>|<span data-ttu-id="2972d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2972d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2972d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2972d-125">Request body</span></span>
<span data-ttu-id="2972d-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="2972d-126">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="2972d-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2972d-127">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="2972d-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2972d-128">Property</span></span>|<span data-ttu-id="2972d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2972d-129">Type</span></span>|<span data-ttu-id="2972d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2972d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2972d-131">id</span><span class="sxs-lookup"><span data-stu-id="2972d-131">id</span></span>|<span data-ttu-id="2972d-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2972d-132">String</span></span>|<span data-ttu-id="2972d-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2972d-133">Key of the entity.</span></span>|
|<span data-ttu-id="2972d-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2972d-134">userDisplayName</span></span>|<span data-ttu-id="2972d-135">String</span><span class="sxs-lookup"><span data-stu-id="2972d-135">String</span></span>|<span data-ttu-id="2972d-136">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="2972d-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="2972d-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="2972d-137">devicesCount</span></span>|<span data-ttu-id="2972d-138">Int32</span><span class="sxs-lookup"><span data-stu-id="2972d-138">Int32</span></span>|<span data-ttu-id="2972d-139">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="2972d-139">Devices count for that user.</span></span>|
|<span data-ttu-id="2972d-140">status</span><span class="sxs-lookup"><span data-stu-id="2972d-140">status</span></span>|[<span data-ttu-id="2972d-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2972d-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2972d-142">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="2972d-142">Compliance status of the policy report.</span></span> <span data-ttu-id="2972d-143">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="2972d-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2972d-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2972d-144">lastReportedDateTime</span></span>|<span data-ttu-id="2972d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2972d-145">DateTimeOffset</span></span>|<span data-ttu-id="2972d-146">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="2972d-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="2972d-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2972d-147">userPrincipalName</span></span>|<span data-ttu-id="2972d-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2972d-148">String</span></span>|<span data-ttu-id="2972d-149">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="2972d-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="2972d-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="2972d-150">Response</span></span>
<span data-ttu-id="2972d-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2972d-151">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2972d-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2972d-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="2972d-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2972d-153">Request</span></span>
<span data-ttu-id="2972d-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2972d-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="2972d-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="2972d-155">Response</span></span>
<span data-ttu-id="2972d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2972d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



