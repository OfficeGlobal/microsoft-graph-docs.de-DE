---
title: deviceManagementPartner erstellen
description: Erstellen eines neuen deviceManagementPartner-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e343b507d81d4d33ca61845e5e9810a09ca700b6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412772"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="4d227-103">deviceManagementPartner erstellen</span><span class="sxs-lookup"><span data-stu-id="4d227-103">Create deviceManagementPartner</span></span>

> <span data-ttu-id="4d227-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="4d227-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4d227-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4d227-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d227-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4d227-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d227-107">Erstellen eines neuen [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4d227-107">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d227-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4d227-108">Prerequisites</span></span>
<span data-ttu-id="4d227-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4d227-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4d227-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d227-111">Permission type</span></span>|<span data-ttu-id="4d227-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d227-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d227-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d227-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d227-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d227-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4d227-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d227-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d227-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d227-116">Not supported.</span></span>|
|<span data-ttu-id="4d227-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d227-117">Application</span></span>|<span data-ttu-id="4d227-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d227-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d227-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d227-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="4d227-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d227-120">Request headers</span></span>
|<span data-ttu-id="4d227-121">Header</span><span class="sxs-lookup"><span data-stu-id="4d227-121">Header</span></span>|<span data-ttu-id="4d227-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4d227-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d227-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4d227-123">Authorization</span></span>|<span data-ttu-id="4d227-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d227-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d227-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4d227-125">Accept</span></span>|<span data-ttu-id="4d227-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d227-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d227-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d227-127">Request body</span></span>
<span data-ttu-id="4d227-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceManagementPartner an.</span><span class="sxs-lookup"><span data-stu-id="4d227-128">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="4d227-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceManagementPartner erstellen.</span><span class="sxs-lookup"><span data-stu-id="4d227-129">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="4d227-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d227-130">Property</span></span>|<span data-ttu-id="4d227-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4d227-131">Type</span></span>|<span data-ttu-id="4d227-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d227-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d227-133">id</span><span class="sxs-lookup"><span data-stu-id="4d227-133">id</span></span>|<span data-ttu-id="4d227-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d227-134">String</span></span>|<span data-ttu-id="4d227-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4d227-135">Not yet documented</span></span>|
|<span data-ttu-id="4d227-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="4d227-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="4d227-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d227-137">DateTimeOffset</span></span>|<span data-ttu-id="4d227-138">Zeitstempel des letzten Heartbeats nach Aktivierung der Option „Connect to Device management Partner“ durch den Administrator</span><span class="sxs-lookup"><span data-stu-id="4d227-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="4d227-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="4d227-139">partnerState</span></span>|[<span data-ttu-id="4d227-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="4d227-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="4d227-141">Partner-Status, der diesen Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4d227-141">Partner state of this tenant.</span></span> <span data-ttu-id="4d227-142">Mögliche Werte sind: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="4d227-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="4d227-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="4d227-143">partnerAppType</span></span>|[<span data-ttu-id="4d227-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="4d227-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="4d227-145">Partner-App-Typ.</span><span class="sxs-lookup"><span data-stu-id="4d227-145">Partner App type.</span></span> <span data-ttu-id="4d227-146">Mögliche Werte sind: `unknown`, `singleTenantApp` und `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="4d227-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="4d227-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="4d227-147">singleTenantAppId</span></span>|<span data-ttu-id="4d227-148">String</span><span class="sxs-lookup"><span data-stu-id="4d227-148">String</span></span>|<span data-ttu-id="4d227-149">ID der Partner-App mit einem einzelnen Mandanten</span><span class="sxs-lookup"><span data-stu-id="4d227-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="4d227-150">displayName</span><span class="sxs-lookup"><span data-stu-id="4d227-150">displayName</span></span>|<span data-ttu-id="4d227-151">String</span><span class="sxs-lookup"><span data-stu-id="4d227-151">String</span></span>|<span data-ttu-id="4d227-152">Anzeigename für Partner</span><span class="sxs-lookup"><span data-stu-id="4d227-152">Partner display name</span></span>|
|<span data-ttu-id="4d227-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="4d227-153">isConfigured</span></span>|<span data-ttu-id="4d227-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d227-154">Boolean</span></span>|<span data-ttu-id="4d227-155">Gibt an, ob Geräteverwaltungspartner konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="4d227-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="4d227-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="4d227-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="4d227-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d227-157">DateTimeOffset</span></span>|<span data-ttu-id="4d227-158">DateTime in UTC beim PartnerDevices entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="4d227-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="4d227-159">Dies wird bald veraltet.</span><span class="sxs-lookup"><span data-stu-id="4d227-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="4d227-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="4d227-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="4d227-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d227-161">DateTimeOffset</span></span>|<span data-ttu-id="4d227-162">DateTime in UTC beim PartnerDevices als nicht kompatibel gekennzeichnet wird.</span><span class="sxs-lookup"><span data-stu-id="4d227-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="4d227-163">Dies wird bald veraltet.</span><span class="sxs-lookup"><span data-stu-id="4d227-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="4d227-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d227-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="4d227-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d227-165">DateTimeOffset</span></span>|<span data-ttu-id="4d227-166">DateTime in UTC, zu der PartnerDevices entfernt werden</span><span class="sxs-lookup"><span data-stu-id="4d227-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="4d227-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="4d227-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="4d227-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d227-168">DateTimeOffset</span></span>|<span data-ttu-id="4d227-169">DateTime in UTC, zu der PartnerDevices als nicht kompatibel gekennzeichnet werden</span><span class="sxs-lookup"><span data-stu-id="4d227-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="4d227-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d227-170">Response</span></span>
<span data-ttu-id="4d227-171">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d227-171">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d227-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d227-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d227-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d227-173">Request</span></span>
<span data-ttu-id="4d227-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d227-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4d227-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d227-175">Response</span></span>
<span data-ttu-id="4d227-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d227-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




