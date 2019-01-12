---
title: deviceManagementPartner aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementPartner-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 068a0ffb3c0411a238a803f3876874f8902e3b35
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981861"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="e377e-103">deviceManagementPartner aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e377e-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="e377e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e377e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e377e-105">Aktualisieren der Eigenschaften eines [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e377e-105">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e377e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e377e-106">Prerequisites</span></span>
<span data-ttu-id="e377e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e377e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e377e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e377e-109">Permission type</span></span>|<span data-ttu-id="e377e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e377e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e377e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e377e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e377e-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e377e-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e377e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e377e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e377e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e377e-114">Not supported.</span></span>|
|<span data-ttu-id="e377e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e377e-115">Application</span></span>|<span data-ttu-id="e377e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e377e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e377e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e377e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="e377e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e377e-118">Request headers</span></span>
|<span data-ttu-id="e377e-119">Header</span><span class="sxs-lookup"><span data-stu-id="e377e-119">Header</span></span>|<span data-ttu-id="e377e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e377e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e377e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e377e-121">Authorization</span></span>|<span data-ttu-id="e377e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e377e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e377e-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e377e-123">Accept</span></span>|<span data-ttu-id="e377e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e377e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e377e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e377e-125">Request body</span></span>
<span data-ttu-id="e377e-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) an.</span><span class="sxs-lookup"><span data-stu-id="e377e-126">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="e377e-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="e377e-127">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="e377e-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e377e-128">Property</span></span>|<span data-ttu-id="e377e-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e377e-129">Type</span></span>|<span data-ttu-id="e377e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e377e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e377e-131">id</span><span class="sxs-lookup"><span data-stu-id="e377e-131">id</span></span>|<span data-ttu-id="e377e-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e377e-132">String</span></span>|<span data-ttu-id="e377e-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e377e-133">Not yet documented</span></span>|
|<span data-ttu-id="e377e-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="e377e-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="e377e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e377e-135">DateTimeOffset</span></span>|<span data-ttu-id="e377e-136">Zeitstempel des letzten Heartbeats nach Aktivierung der Option „Connect to Device management Partner“ durch den Administrator</span><span class="sxs-lookup"><span data-stu-id="e377e-136">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="e377e-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="e377e-137">partnerState</span></span>|[<span data-ttu-id="e377e-138">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="e377e-138">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="e377e-139">Partner-Status, der diesen Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e377e-139">Partner state of this tenant.</span></span> <span data-ttu-id="e377e-140">Mögliche Werte sind: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="e377e-140">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="e377e-141">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="e377e-141">partnerAppType</span></span>|[<span data-ttu-id="e377e-142">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="e377e-142">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="e377e-143">Partner-App-Typ.</span><span class="sxs-lookup"><span data-stu-id="e377e-143">Partner App type.</span></span> <span data-ttu-id="e377e-144">Mögliche Werte sind: `unknown`, `singleTenantApp` und `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="e377e-144">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="e377e-145">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="e377e-145">singleTenantAppId</span></span>|<span data-ttu-id="e377e-146">String</span><span class="sxs-lookup"><span data-stu-id="e377e-146">String</span></span>|<span data-ttu-id="e377e-147">ID der Partner-App mit einem einzelnen Mandanten</span><span class="sxs-lookup"><span data-stu-id="e377e-147">Partner Single tenant App id</span></span>|
|<span data-ttu-id="e377e-148">displayName</span><span class="sxs-lookup"><span data-stu-id="e377e-148">displayName</span></span>|<span data-ttu-id="e377e-149">String</span><span class="sxs-lookup"><span data-stu-id="e377e-149">String</span></span>|<span data-ttu-id="e377e-150">Anzeigename für Partner</span><span class="sxs-lookup"><span data-stu-id="e377e-150">Partner display name</span></span>|
|<span data-ttu-id="e377e-151">isConfigured</span><span class="sxs-lookup"><span data-stu-id="e377e-151">isConfigured</span></span>|<span data-ttu-id="e377e-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e377e-152">Boolean</span></span>|<span data-ttu-id="e377e-153">Gibt an, ob Geräteverwaltungspartner konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="e377e-153">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="e377e-154">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="e377e-154">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="e377e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e377e-155">DateTimeOffset</span></span>|<span data-ttu-id="e377e-156">DateTime in UTC, zu der PartnerDevices entfernt werden</span><span class="sxs-lookup"><span data-stu-id="e377e-156">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="e377e-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="e377e-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="e377e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e377e-158">DateTimeOffset</span></span>|<span data-ttu-id="e377e-159">DateTime in UTC, zu der PartnerDevices als nicht kompatibel gekennzeichnet werden</span><span class="sxs-lookup"><span data-stu-id="e377e-159">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="e377e-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="e377e-160">Response</span></span>
<span data-ttu-id="e377e-161">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e377e-161">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e377e-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e377e-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="e377e-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e377e-163">Request</span></span>
<span data-ttu-id="e377e-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e377e-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 502

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e377e-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="e377e-165">Response</span></span>
<span data-ttu-id="e377e-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e377e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 551

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```



