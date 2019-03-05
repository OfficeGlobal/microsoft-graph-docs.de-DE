---
title: deviceManagementPartner erstellen
description: Erstellen eines neuen deviceManagementPartner-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b26522e88b50230e4636dac9dc4bb832830d138
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143225"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="869e8-103">deviceManagementPartner erstellen</span><span class="sxs-lookup"><span data-stu-id="869e8-103">Create deviceManagementPartner</span></span>

> <span data-ttu-id="869e8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="869e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="869e8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="869e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="869e8-106">Erstellen eines neuen [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="869e8-106">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="869e8-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="869e8-107">Prerequisites</span></span>
<span data-ttu-id="869e8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="869e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="869e8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="869e8-110">Permission type</span></span>|<span data-ttu-id="869e8-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="869e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="869e8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="869e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="869e8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="869e8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="869e8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="869e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="869e8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="869e8-115">Not supported.</span></span>|
|<span data-ttu-id="869e8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="869e8-116">Application</span></span>|<span data-ttu-id="869e8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="869e8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="869e8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="869e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="869e8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="869e8-119">Request headers</span></span>
|<span data-ttu-id="869e8-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="869e8-120">Header</span></span>|<span data-ttu-id="869e8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="869e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="869e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="869e8-122">Authorization</span></span>|<span data-ttu-id="869e8-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="869e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="869e8-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="869e8-124">Accept</span></span>|<span data-ttu-id="869e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="869e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="869e8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="869e8-126">Request body</span></span>
<span data-ttu-id="869e8-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementPartner an.</span><span class="sxs-lookup"><span data-stu-id="869e8-127">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="869e8-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementPartner erstellen.</span><span class="sxs-lookup"><span data-stu-id="869e8-128">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="869e8-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="869e8-129">Property</span></span>|<span data-ttu-id="869e8-130">Typ</span><span class="sxs-lookup"><span data-stu-id="869e8-130">Type</span></span>|<span data-ttu-id="869e8-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="869e8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="869e8-132">id</span><span class="sxs-lookup"><span data-stu-id="869e8-132">id</span></span>|<span data-ttu-id="869e8-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="869e8-133">String</span></span>|<span data-ttu-id="869e8-134">ID der Entität</span><span class="sxs-lookup"><span data-stu-id="869e8-134">Id of the entity</span></span>|
|<span data-ttu-id="869e8-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="869e8-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="869e8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="869e8-136">DateTimeOffset</span></span>|<span data-ttu-id="869e8-137">Zeitstempel des letzten Heartbeats nach Aktivierung der Option „Connect to Device management Partner“ durch den Administrator</span><span class="sxs-lookup"><span data-stu-id="869e8-137">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="869e8-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="869e8-138">partnerState</span></span>|[<span data-ttu-id="869e8-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="869e8-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="869e8-140">Partner Status dieses Mandanten.</span><span class="sxs-lookup"><span data-stu-id="869e8-140">Partner state of this tenant.</span></span> <span data-ttu-id="869e8-141">Mögliche Werte sind: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="869e8-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="869e8-142">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="869e8-142">partnerAppType</span></span>|[<span data-ttu-id="869e8-143">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="869e8-143">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="869e8-144">Partner-App-Typ.</span><span class="sxs-lookup"><span data-stu-id="869e8-144">Partner App type.</span></span> <span data-ttu-id="869e8-145">Mögliche Werte sind: `unknown`, `singleTenantApp` und `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="869e8-145">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="869e8-146">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="869e8-146">singleTenantAppId</span></span>|<span data-ttu-id="869e8-147">String</span><span class="sxs-lookup"><span data-stu-id="869e8-147">String</span></span>|<span data-ttu-id="869e8-148">ID der Partner-App mit einem einzelnen Mandanten</span><span class="sxs-lookup"><span data-stu-id="869e8-148">Partner Single tenant App id</span></span>|
|<span data-ttu-id="869e8-149">displayName</span><span class="sxs-lookup"><span data-stu-id="869e8-149">displayName</span></span>|<span data-ttu-id="869e8-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="869e8-150">String</span></span>|<span data-ttu-id="869e8-151">Anzeigename für Partner</span><span class="sxs-lookup"><span data-stu-id="869e8-151">Partner display name</span></span>|
|<span data-ttu-id="869e8-152">isConfigured</span><span class="sxs-lookup"><span data-stu-id="869e8-152">isConfigured</span></span>|<span data-ttu-id="869e8-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="869e8-153">Boolean</span></span>|<span data-ttu-id="869e8-154">Gibt an, ob Geräteverwaltungspartner konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="869e8-154">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="869e8-155">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="869e8-155">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="869e8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="869e8-156">DateTimeOffset</span></span>|<span data-ttu-id="869e8-157">DateTime in UTC, wenn PartnerDevices entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="869e8-157">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="869e8-158">Dies wird bald Obselete.</span><span class="sxs-lookup"><span data-stu-id="869e8-158">This will become obselete soon.</span></span>|
|<span data-ttu-id="869e8-159">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="869e8-159">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="869e8-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="869e8-160">DateTimeOffset</span></span>|<span data-ttu-id="869e8-161">DateTime in UTC, wenn PartnerDevices als nicht kompatibel gekennzeichnet wird.</span><span class="sxs-lookup"><span data-stu-id="869e8-161">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="869e8-162">Dies wird bald Obselete.</span><span class="sxs-lookup"><span data-stu-id="869e8-162">This will become obselete soon.</span></span>|
|<span data-ttu-id="869e8-163">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="869e8-163">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="869e8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="869e8-164">DateTimeOffset</span></span>|<span data-ttu-id="869e8-165">DateTime in UTC, zu der PartnerDevices entfernt werden</span><span class="sxs-lookup"><span data-stu-id="869e8-165">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="869e8-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="869e8-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="869e8-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="869e8-167">DateTimeOffset</span></span>|<span data-ttu-id="869e8-168">DateTime in UTC, zu der PartnerDevices als nicht kompatibel gekennzeichnet werden</span><span class="sxs-lookup"><span data-stu-id="869e8-168">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="869e8-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="869e8-169">Response</span></span>
<span data-ttu-id="869e8-170">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="869e8-170">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="869e8-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="869e8-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="869e8-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="869e8-172">Request</span></span>
<span data-ttu-id="869e8-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="869e8-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
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

### <a name="response"></a><span data-ttu-id="869e8-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="869e8-174">Response</span></span>
<span data-ttu-id="869e8-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="869e8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




