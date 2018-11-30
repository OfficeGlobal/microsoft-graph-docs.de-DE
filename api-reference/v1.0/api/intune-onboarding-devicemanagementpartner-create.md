---
title: deviceManagementPartner erstellen
description: Erstellen eines neuen deviceManagementPartner-Objekts.
ms.openlocfilehash: 038bfecf443972921c7aeacc508e9b1b81331cf4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019169"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="c89d9-103">deviceManagementPartner erstellen</span><span class="sxs-lookup"><span data-stu-id="c89d9-103">Create deviceManagementPartner</span></span>

> <span data-ttu-id="c89d9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c89d9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c89d9-105">Erstellen eines neuen [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c89d9-105">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c89d9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c89d9-106">Prerequisites</span></span>
<span data-ttu-id="c89d9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c89d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c89d9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c89d9-109">Permission type</span></span>|<span data-ttu-id="c89d9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c89d9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c89d9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c89d9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c89d9-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c89d9-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c89d9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c89d9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c89d9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c89d9-114">Not supported.</span></span>|
|<span data-ttu-id="c89d9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c89d9-115">Application</span></span>|<span data-ttu-id="c89d9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c89d9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c89d9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c89d9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="c89d9-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c89d9-118">Request headers</span></span>
|<span data-ttu-id="c89d9-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c89d9-119">Header</span></span>|<span data-ttu-id="c89d9-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c89d9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c89d9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c89d9-121">Authorization</span></span>|<span data-ttu-id="c89d9-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c89d9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c89d9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c89d9-123">Accept</span></span>|<span data-ttu-id="c89d9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c89d9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c89d9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c89d9-125">Request body</span></span>
<span data-ttu-id="c89d9-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementPartner an.</span><span class="sxs-lookup"><span data-stu-id="c89d9-126">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="c89d9-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementPartner erstellen.</span><span class="sxs-lookup"><span data-stu-id="c89d9-127">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="c89d9-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c89d9-128">Property</span></span>|<span data-ttu-id="c89d9-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c89d9-129">Type</span></span>|<span data-ttu-id="c89d9-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c89d9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c89d9-131">id</span><span class="sxs-lookup"><span data-stu-id="c89d9-131">id</span></span>|<span data-ttu-id="c89d9-132">String</span><span class="sxs-lookup"><span data-stu-id="c89d9-132">String</span></span>|<span data-ttu-id="c89d9-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c89d9-133">Not yet documented</span></span>|
|<span data-ttu-id="c89d9-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="c89d9-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="c89d9-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c89d9-135">DateTimeOffset</span></span>|<span data-ttu-id="c89d9-136">Zeitstempel des letzten Heartbeats nach Aktivierung der Option „Connect to Device management Partner“ durch den Administrator</span><span class="sxs-lookup"><span data-stu-id="c89d9-136">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="c89d9-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="c89d9-137">partnerState</span></span>|[<span data-ttu-id="c89d9-138">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="c89d9-138">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="c89d9-139">Partner-Status, der diesen Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c89d9-139">Partner state of this tenant.</span></span> <span data-ttu-id="c89d9-140">Mögliche Werte sind: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="c89d9-140">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="c89d9-141">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="c89d9-141">partnerAppType</span></span>|[<span data-ttu-id="c89d9-142">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="c89d9-142">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="c89d9-143">Partner-App-Typ.</span><span class="sxs-lookup"><span data-stu-id="c89d9-143">Partner App type.</span></span> <span data-ttu-id="c89d9-144">Mögliche Werte sind: `unknown`, `singleTenantApp` und `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="c89d9-144">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="c89d9-145">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="c89d9-145">singleTenantAppId</span></span>|<span data-ttu-id="c89d9-146">String</span><span class="sxs-lookup"><span data-stu-id="c89d9-146">String</span></span>|<span data-ttu-id="c89d9-147">ID der Partner-App mit einem einzelnen Mandanten</span><span class="sxs-lookup"><span data-stu-id="c89d9-147">Partner Single tenant App id</span></span>|
|<span data-ttu-id="c89d9-148">displayName</span><span class="sxs-lookup"><span data-stu-id="c89d9-148">displayName</span></span>|<span data-ttu-id="c89d9-149">String</span><span class="sxs-lookup"><span data-stu-id="c89d9-149">String</span></span>|<span data-ttu-id="c89d9-150">Anzeigename für Partner</span><span class="sxs-lookup"><span data-stu-id="c89d9-150">Partner display name</span></span>|
|<span data-ttu-id="c89d9-151">isConfigured</span><span class="sxs-lookup"><span data-stu-id="c89d9-151">isConfigured</span></span>|<span data-ttu-id="c89d9-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c89d9-152">Boolean</span></span>|<span data-ttu-id="c89d9-153">Gibt an, ob Geräteverwaltungspartner konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="c89d9-153">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="c89d9-154">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="c89d9-154">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="c89d9-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c89d9-155">DateTimeOffset</span></span>|<span data-ttu-id="c89d9-156">DateTime in UTC, zu der PartnerDevices entfernt werden</span><span class="sxs-lookup"><span data-stu-id="c89d9-156">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="c89d9-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="c89d9-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="c89d9-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c89d9-158">DateTimeOffset</span></span>|<span data-ttu-id="c89d9-159">DateTime in UTC, zu der PartnerDevices als nicht kompatibel gekennzeichnet werden</span><span class="sxs-lookup"><span data-stu-id="c89d9-159">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="c89d9-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="c89d9-160">Response</span></span>
<span data-ttu-id="c89d9-161">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c89d9-161">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c89d9-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c89d9-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="c89d9-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c89d9-163">Request</span></span>
<span data-ttu-id="c89d9-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c89d9-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
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

### <a name="response"></a><span data-ttu-id="c89d9-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="c89d9-165">Response</span></span>
<span data-ttu-id="c89d9-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c89d9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



