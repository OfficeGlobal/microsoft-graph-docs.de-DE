---
title: deviceManagementPartner aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementPartner-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 26646fc7afb04fb577f8cbf7d160869de8889e65
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956444"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="53406-103">deviceManagementPartner aktualisieren</span><span class="sxs-lookup"><span data-stu-id="53406-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="53406-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="53406-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53406-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="53406-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53406-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="53406-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53406-107">Aktualisieren der Eigenschaften eines [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="53406-107">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53406-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="53406-108">Prerequisites</span></span>
<span data-ttu-id="53406-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53406-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53406-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53406-111">Permission type</span></span>|<span data-ttu-id="53406-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53406-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53406-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53406-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53406-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53406-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="53406-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53406-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53406-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53406-116">Not supported.</span></span>|
|<span data-ttu-id="53406-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53406-117">Application</span></span>|<span data-ttu-id="53406-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53406-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53406-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53406-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="53406-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53406-120">Request headers</span></span>
|<span data-ttu-id="53406-121">Header</span><span class="sxs-lookup"><span data-stu-id="53406-121">Header</span></span>|<span data-ttu-id="53406-122">Wert</span><span class="sxs-lookup"><span data-stu-id="53406-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53406-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53406-123">Authorization</span></span>|<span data-ttu-id="53406-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="53406-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53406-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="53406-125">Accept</span></span>|<span data-ttu-id="53406-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53406-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53406-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53406-127">Request body</span></span>
<span data-ttu-id="53406-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) an.</span><span class="sxs-lookup"><span data-stu-id="53406-128">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="53406-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="53406-129">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="53406-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="53406-130">Property</span></span>|<span data-ttu-id="53406-131">Typ</span><span class="sxs-lookup"><span data-stu-id="53406-131">Type</span></span>|<span data-ttu-id="53406-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53406-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53406-133">id</span><span class="sxs-lookup"><span data-stu-id="53406-133">id</span></span>|<span data-ttu-id="53406-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="53406-134">String</span></span>|<span data-ttu-id="53406-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="53406-135">Not yet documented</span></span>|
|<span data-ttu-id="53406-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="53406-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="53406-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53406-137">DateTimeOffset</span></span>|<span data-ttu-id="53406-138">Zeitstempel des letzten Heartbeats nach Aktivierung der Option „Connect to Device management Partner“ durch den Administrator</span><span class="sxs-lookup"><span data-stu-id="53406-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="53406-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="53406-139">partnerState</span></span>|[<span data-ttu-id="53406-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="53406-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="53406-141">Partner-Status, der diesen Mandanten.</span><span class="sxs-lookup"><span data-stu-id="53406-141">Partner state of this tenant.</span></span> <span data-ttu-id="53406-142">Mögliche Werte sind: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="53406-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="53406-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="53406-143">partnerAppType</span></span>|[<span data-ttu-id="53406-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="53406-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="53406-145">Partner-App-Typ.</span><span class="sxs-lookup"><span data-stu-id="53406-145">Partner App type.</span></span> <span data-ttu-id="53406-146">Mögliche Werte sind: `unknown`, `singleTenantApp` und `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="53406-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="53406-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="53406-147">singleTenantAppId</span></span>|<span data-ttu-id="53406-148">String</span><span class="sxs-lookup"><span data-stu-id="53406-148">String</span></span>|<span data-ttu-id="53406-149">ID der Partner-App mit einem einzelnen Mandanten</span><span class="sxs-lookup"><span data-stu-id="53406-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="53406-150">displayName</span><span class="sxs-lookup"><span data-stu-id="53406-150">displayName</span></span>|<span data-ttu-id="53406-151">String</span><span class="sxs-lookup"><span data-stu-id="53406-151">String</span></span>|<span data-ttu-id="53406-152">Anzeigename für Partner</span><span class="sxs-lookup"><span data-stu-id="53406-152">Partner display name</span></span>|
|<span data-ttu-id="53406-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="53406-153">isConfigured</span></span>|<span data-ttu-id="53406-154">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="53406-154">Boolean</span></span>|<span data-ttu-id="53406-155">Gibt an, ob Geräteverwaltungspartner konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="53406-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="53406-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="53406-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="53406-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53406-157">DateTimeOffset</span></span>|<span data-ttu-id="53406-158">DateTime in UTC beim PartnerDevices entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="53406-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="53406-159">Dies wird bald veraltet.</span><span class="sxs-lookup"><span data-stu-id="53406-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="53406-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="53406-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="53406-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53406-161">DateTimeOffset</span></span>|<span data-ttu-id="53406-162">DateTime in UTC beim PartnerDevices als nicht kompatibel gekennzeichnet wird.</span><span class="sxs-lookup"><span data-stu-id="53406-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="53406-163">Dies wird bald veraltet.</span><span class="sxs-lookup"><span data-stu-id="53406-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="53406-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="53406-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="53406-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53406-165">DateTimeOffset</span></span>|<span data-ttu-id="53406-166">DateTime in UTC, zu der PartnerDevices entfernt werden</span><span class="sxs-lookup"><span data-stu-id="53406-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="53406-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="53406-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="53406-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53406-168">DateTimeOffset</span></span>|<span data-ttu-id="53406-169">DateTime in UTC, zu der PartnerDevices als nicht kompatibel gekennzeichnet werden</span><span class="sxs-lookup"><span data-stu-id="53406-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="53406-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="53406-170">Response</span></span>
<span data-ttu-id="53406-171">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53406-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53406-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53406-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="53406-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53406-173">Request</span></span>
<span data-ttu-id="53406-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53406-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 602

{
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

### <a name="response"></a><span data-ttu-id="53406-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="53406-175">Response</span></span>
<span data-ttu-id="53406-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53406-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





