---
title: Aktualisieren von „managedDeviceMobileAppConfigurationUserStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceMobileAppConfigurationUserStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05ea762bafe2d5a950c4d5e582ec4e185f6d2425
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405156"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="4fc0f-103">Aktualisieren von „managedDeviceMobileAppConfigurationUserStatus“</span><span class="sxs-lookup"><span data-stu-id="4fc0f-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="4fc0f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="4fc0f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4fc0f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4fc0f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4fc0f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4fc0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fc0f-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="4fc0f-107">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fc0f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4fc0f-108">Prerequisites</span></span>
<span data-ttu-id="4fc0f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4fc0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4fc0f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4fc0f-111">Permission type</span></span>|<span data-ttu-id="4fc0f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4fc0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fc0f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4fc0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4fc0f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fc0f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4fc0f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4fc0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fc0f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4fc0f-116">Not supported.</span></span>|
|<span data-ttu-id="4fc0f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4fc0f-117">Application</span></span>|<span data-ttu-id="4fc0f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4fc0f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fc0f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4fc0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="4fc0f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4fc0f-120">Request headers</span></span>
|<span data-ttu-id="4fc0f-121">Header</span><span class="sxs-lookup"><span data-stu-id="4fc0f-121">Header</span></span>|<span data-ttu-id="4fc0f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4fc0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fc0f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4fc0f-123">Authorization</span></span>|<span data-ttu-id="4fc0f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4fc0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fc0f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4fc0f-125">Accept</span></span>|<span data-ttu-id="4fc0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4fc0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fc0f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4fc0f-127">Request body</span></span>
<span data-ttu-id="4fc0f-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="4fc0f-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="4fc0f-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="4fc0f-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="4fc0f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4fc0f-130">Property</span></span>|<span data-ttu-id="4fc0f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4fc0f-131">Type</span></span>|<span data-ttu-id="4fc0f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4fc0f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fc0f-133">id</span><span class="sxs-lookup"><span data-stu-id="4fc0f-133">id</span></span>|<span data-ttu-id="4fc0f-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4fc0f-134">String</span></span>|<span data-ttu-id="4fc0f-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4fc0f-135">Key of the entity.</span></span>|
|<span data-ttu-id="4fc0f-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4fc0f-136">userDisplayName</span></span>|<span data-ttu-id="4fc0f-137">String</span><span class="sxs-lookup"><span data-stu-id="4fc0f-137">String</span></span>|<span data-ttu-id="4fc0f-138">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="4fc0f-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="4fc0f-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="4fc0f-139">devicesCount</span></span>|<span data-ttu-id="4fc0f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4fc0f-140">Int32</span></span>|<span data-ttu-id="4fc0f-141">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="4fc0f-141">Devices count for that user.</span></span>|
|<span data-ttu-id="4fc0f-142">status</span><span class="sxs-lookup"><span data-stu-id="4fc0f-142">status</span></span>|[<span data-ttu-id="4fc0f-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4fc0f-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4fc0f-144">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="4fc0f-144">Compliance status of the policy report.</span></span> <span data-ttu-id="4fc0f-145">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="4fc0f-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4fc0f-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4fc0f-146">lastReportedDateTime</span></span>|<span data-ttu-id="4fc0f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fc0f-147">DateTimeOffset</span></span>|<span data-ttu-id="4fc0f-148">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="4fc0f-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="4fc0f-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4fc0f-149">userPrincipalName</span></span>|<span data-ttu-id="4fc0f-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4fc0f-150">String</span></span>|<span data-ttu-id="4fc0f-151">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="4fc0f-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="4fc0f-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="4fc0f-152">Response</span></span>
<span data-ttu-id="4fc0f-153">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4fc0f-153">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fc0f-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4fc0f-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fc0f-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4fc0f-155">Request</span></span>
<span data-ttu-id="4fc0f-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4fc0f-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="4fc0f-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="4fc0f-157">Response</span></span>
<span data-ttu-id="4fc0f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4fc0f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "44960944-0944-4496-4409-964444099644",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




