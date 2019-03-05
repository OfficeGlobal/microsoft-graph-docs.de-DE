---
title: Erstellen von „managedDeviceMobileAppConfigurationUserStatus“
description: Diese Methode erstellt ein neues Objekt des Typs managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da46008eee715c7ecff2057015cb0dacb37102b7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251447"
---
# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="a15d6-103">Erstellen von „managedDeviceMobileAppConfigurationUserStatus“</span><span class="sxs-lookup"><span data-stu-id="a15d6-103">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="a15d6-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a15d6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a15d6-105">Diese Methode erstellt ein neues Objekt des Typs [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a15d6-105">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a15d6-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a15d6-106">Prerequisites</span></span>
<span data-ttu-id="a15d6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a15d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a15d6-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a15d6-109">Permission type</span></span>|<span data-ttu-id="a15d6-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a15d6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a15d6-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a15d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a15d6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a15d6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a15d6-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a15d6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a15d6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a15d6-114">Not supported.</span></span>|
|<span data-ttu-id="a15d6-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a15d6-115">Application</span></span>|<span data-ttu-id="a15d6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a15d6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a15d6-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a15d6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a15d6-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a15d6-118">Request headers</span></span>
|<span data-ttu-id="a15d6-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a15d6-119">Header</span></span>|<span data-ttu-id="a15d6-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a15d6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a15d6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a15d6-121">Authorization</span></span>|<span data-ttu-id="a15d6-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a15d6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a15d6-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a15d6-123">Accept</span></span>|<span data-ttu-id="a15d6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a15d6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a15d6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a15d6-125">Request body</span></span>
<span data-ttu-id="a15d6-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedDeviceMobileAppConfigurationUserStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="a15d6-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationUserStatus object.</span></span>

<span data-ttu-id="a15d6-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedDeviceMobileAppConfigurationUserStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="a15d6-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationUserStatus.</span></span>

|<span data-ttu-id="a15d6-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a15d6-128">Property</span></span>|<span data-ttu-id="a15d6-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a15d6-129">Type</span></span>|<span data-ttu-id="a15d6-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a15d6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a15d6-131">id</span><span class="sxs-lookup"><span data-stu-id="a15d6-131">id</span></span>|<span data-ttu-id="a15d6-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a15d6-132">String</span></span>|<span data-ttu-id="a15d6-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a15d6-133">Key of the entity.</span></span>|
|<span data-ttu-id="a15d6-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a15d6-134">userDisplayName</span></span>|<span data-ttu-id="a15d6-135">String</span><span class="sxs-lookup"><span data-stu-id="a15d6-135">String</span></span>|<span data-ttu-id="a15d6-136">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="a15d6-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="a15d6-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="a15d6-137">devicesCount</span></span>|<span data-ttu-id="a15d6-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a15d6-138">Int32</span></span>|<span data-ttu-id="a15d6-139">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="a15d6-139">Devices count for that user.</span></span>|
|<span data-ttu-id="a15d6-140">status</span><span class="sxs-lookup"><span data-stu-id="a15d6-140">status</span></span>|[<span data-ttu-id="a15d6-141">Wurde</span><span class="sxs-lookup"><span data-stu-id="a15d6-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a15d6-142">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="a15d6-142">Compliance status of the policy report.</span></span> <span data-ttu-id="a15d6-143">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a15d6-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a15d6-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a15d6-144">lastReportedDateTime</span></span>|<span data-ttu-id="a15d6-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a15d6-145">DateTimeOffset</span></span>|<span data-ttu-id="a15d6-146">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="a15d6-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="a15d6-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a15d6-147">userPrincipalName</span></span>|<span data-ttu-id="a15d6-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a15d6-148">String</span></span>|<span data-ttu-id="a15d6-149">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="a15d6-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="a15d6-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="a15d6-150">Response</span></span>
<span data-ttu-id="a15d6-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a15d6-151">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a15d6-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a15d6-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="a15d6-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a15d6-153">Request</span></span>
<span data-ttu-id="a15d6-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a15d6-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="a15d6-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="a15d6-155">Response</span></span>
<span data-ttu-id="a15d6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a15d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



