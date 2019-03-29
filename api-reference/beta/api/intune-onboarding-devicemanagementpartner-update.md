---
title: deviceManagementPartner aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementPartner-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a73b5b9dae8a703f6429916bdaee556511dd624d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981986"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="53444-103">deviceManagementPartner aktualisieren</span><span class="sxs-lookup"><span data-stu-id="53444-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="53444-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="53444-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53444-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="53444-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53444-106">Aktualisieren der Eigenschaften eines [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="53444-106">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53444-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="53444-107">Prerequisites</span></span>
<span data-ttu-id="53444-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53444-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53444-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53444-110">Permission type</span></span>|<span data-ttu-id="53444-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53444-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53444-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53444-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53444-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53444-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="53444-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53444-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53444-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53444-115">Not supported.</span></span>|
|<span data-ttu-id="53444-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53444-116">Application</span></span>|<span data-ttu-id="53444-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53444-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53444-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53444-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="53444-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53444-119">Request headers</span></span>
|<span data-ttu-id="53444-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="53444-120">Header</span></span>|<span data-ttu-id="53444-121">Wert</span><span class="sxs-lookup"><span data-stu-id="53444-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53444-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53444-122">Authorization</span></span>|<span data-ttu-id="53444-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="53444-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53444-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="53444-124">Accept</span></span>|<span data-ttu-id="53444-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53444-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53444-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53444-126">Request body</span></span>
<span data-ttu-id="53444-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) an.</span><span class="sxs-lookup"><span data-stu-id="53444-127">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="53444-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="53444-128">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="53444-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="53444-129">Property</span></span>|<span data-ttu-id="53444-130">Typ</span><span class="sxs-lookup"><span data-stu-id="53444-130">Type</span></span>|<span data-ttu-id="53444-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53444-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53444-132">id</span><span class="sxs-lookup"><span data-stu-id="53444-132">id</span></span>|<span data-ttu-id="53444-133">String</span><span class="sxs-lookup"><span data-stu-id="53444-133">String</span></span>|<span data-ttu-id="53444-134">ID der Entität</span><span class="sxs-lookup"><span data-stu-id="53444-134">Id of the entity</span></span>|
|<span data-ttu-id="53444-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="53444-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="53444-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53444-136">DateTimeOffset</span></span>|<span data-ttu-id="53444-137">Zeitstempel des letzten Heartbeats nach Aktivierung der Option „Connect to Device management Partner“ durch den Administrator</span><span class="sxs-lookup"><span data-stu-id="53444-137">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="53444-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="53444-138">partnerState</span></span>|[<span data-ttu-id="53444-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="53444-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="53444-140">Partner Status dieses Mandanten.</span><span class="sxs-lookup"><span data-stu-id="53444-140">Partner state of this tenant.</span></span> <span data-ttu-id="53444-141">Mögliche Werte sind: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="53444-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="53444-142">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="53444-142">partnerAppType</span></span>|[<span data-ttu-id="53444-143">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="53444-143">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="53444-144">Partner-App-Typ.</span><span class="sxs-lookup"><span data-stu-id="53444-144">Partner App type.</span></span> <span data-ttu-id="53444-145">Mögliche Werte sind: `unknown`, `singleTenantApp` und `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="53444-145">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="53444-146">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="53444-146">singleTenantAppId</span></span>|<span data-ttu-id="53444-147">String</span><span class="sxs-lookup"><span data-stu-id="53444-147">String</span></span>|<span data-ttu-id="53444-148">ID der Partner-App mit einem einzelnen Mandanten</span><span class="sxs-lookup"><span data-stu-id="53444-148">Partner Single tenant App id</span></span>|
|<span data-ttu-id="53444-149">displayName</span><span class="sxs-lookup"><span data-stu-id="53444-149">displayName</span></span>|<span data-ttu-id="53444-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="53444-150">String</span></span>|<span data-ttu-id="53444-151">Anzeigename für Partner</span><span class="sxs-lookup"><span data-stu-id="53444-151">Partner display name</span></span>|
|<span data-ttu-id="53444-152">isConfigured</span><span class="sxs-lookup"><span data-stu-id="53444-152">isConfigured</span></span>|<span data-ttu-id="53444-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="53444-153">Boolean</span></span>|<span data-ttu-id="53444-154">Gibt an, ob Geräteverwaltungspartner konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="53444-154">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="53444-155">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="53444-155">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="53444-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53444-156">DateTimeOffset</span></span>|<span data-ttu-id="53444-157">DateTime in UTC, wenn PartnerDevices entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="53444-157">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="53444-158">Dies wird bald Obselete.</span><span class="sxs-lookup"><span data-stu-id="53444-158">This will become obselete soon.</span></span>|
|<span data-ttu-id="53444-159">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="53444-159">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="53444-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53444-160">DateTimeOffset</span></span>|<span data-ttu-id="53444-161">DateTime in UTC, wenn PartnerDevices als nicht kompatibel gekennzeichnet wird.</span><span class="sxs-lookup"><span data-stu-id="53444-161">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="53444-162">Dies wird bald Obselete.</span><span class="sxs-lookup"><span data-stu-id="53444-162">This will become obselete soon.</span></span>|
|<span data-ttu-id="53444-163">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="53444-163">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="53444-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53444-164">DateTimeOffset</span></span>|<span data-ttu-id="53444-165">DateTime in UTC, zu der PartnerDevices entfernt werden</span><span class="sxs-lookup"><span data-stu-id="53444-165">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="53444-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="53444-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="53444-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53444-167">DateTimeOffset</span></span>|<span data-ttu-id="53444-168">DateTime in UTC, zu der PartnerDevices als nicht kompatibel gekennzeichnet werden</span><span class="sxs-lookup"><span data-stu-id="53444-168">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="53444-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="53444-169">Response</span></span>
<span data-ttu-id="53444-170">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53444-170">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53444-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53444-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="53444-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53444-172">Request</span></span>
<span data-ttu-id="53444-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53444-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 664

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a><span data-ttu-id="53444-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="53444-174">Response</span></span>
<span data-ttu-id="53444-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53444-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 713

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```




