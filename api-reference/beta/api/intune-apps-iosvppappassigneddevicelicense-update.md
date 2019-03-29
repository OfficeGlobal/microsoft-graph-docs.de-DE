---
title: IosVppAppAssignedDeviceLicense aktualisieren
description: Aktualisieren der Eigenschaften eines iosVppAppAssignedDeviceLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 50de14fa5080c41e1636fc385fef057ef6aacac3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981195"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="d5ee9-103">IosVppAppAssignedDeviceLicense aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d5ee9-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="d5ee9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d5ee9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5ee9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d5ee9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5ee9-106">Aktualisieren der Eigenschaften eines [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d5ee9-106">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5ee9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d5ee9-107">Prerequisites</span></span>
<span data-ttu-id="d5ee9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5ee9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5ee9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d5ee9-110">Permission type</span></span>|<span data-ttu-id="d5ee9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d5ee9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5ee9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d5ee9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d5ee9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5ee9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d5ee9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d5ee9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5ee9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5ee9-115">Not supported.</span></span>|
|<span data-ttu-id="d5ee9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d5ee9-116">Application</span></span>|<span data-ttu-id="d5ee9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5ee9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5ee9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5ee9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="d5ee9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d5ee9-119">Request headers</span></span>
|<span data-ttu-id="d5ee9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d5ee9-120">Header</span></span>|<span data-ttu-id="d5ee9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d5ee9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5ee9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5ee9-122">Authorization</span></span>|<span data-ttu-id="d5ee9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d5ee9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5ee9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d5ee9-124">Accept</span></span>|<span data-ttu-id="d5ee9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d5ee9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5ee9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d5ee9-126">Request body</span></span>
<span data-ttu-id="d5ee9-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d5ee9-127">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="d5ee9-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d5ee9-128">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="d5ee9-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d5ee9-129">Property</span></span>|<span data-ttu-id="d5ee9-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d5ee9-130">Type</span></span>|<span data-ttu-id="d5ee9-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d5ee9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5ee9-132">id</span><span class="sxs-lookup"><span data-stu-id="d5ee9-132">id</span></span>|<span data-ttu-id="d5ee9-133">String</span><span class="sxs-lookup"><span data-stu-id="d5ee9-133">String</span></span>|<span data-ttu-id="d5ee9-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d5ee9-134">Key of the entity.</span></span> <span data-ttu-id="d5ee9-135">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d5ee9-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d5ee9-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="d5ee9-136">userEmailAddress</span></span>|<span data-ttu-id="d5ee9-137">String</span><span class="sxs-lookup"><span data-stu-id="d5ee9-137">String</span></span>|<span data-ttu-id="d5ee9-138">Die Benutzer-e-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="d5ee9-138">The user email address.</span></span> <span data-ttu-id="d5ee9-139">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d5ee9-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d5ee9-140">userId</span><span class="sxs-lookup"><span data-stu-id="d5ee9-140">userId</span></span>|<span data-ttu-id="d5ee9-141">String</span><span class="sxs-lookup"><span data-stu-id="d5ee9-141">String</span></span>|<span data-ttu-id="d5ee9-142">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="d5ee9-142">The user ID.</span></span> <span data-ttu-id="d5ee9-143">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d5ee9-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d5ee9-144">userName</span><span class="sxs-lookup"><span data-stu-id="d5ee9-144">userName</span></span>|<span data-ttu-id="d5ee9-145">String</span><span class="sxs-lookup"><span data-stu-id="d5ee9-145">String</span></span>|<span data-ttu-id="d5ee9-146">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="d5ee9-146">The user name.</span></span> <span data-ttu-id="d5ee9-147">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d5ee9-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d5ee9-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d5ee9-148">userPrincipalName</span></span>|<span data-ttu-id="d5ee9-149">String</span><span class="sxs-lookup"><span data-stu-id="d5ee9-149">String</span></span>|<span data-ttu-id="d5ee9-150">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="d5ee9-150">The user principal name.</span></span> <span data-ttu-id="d5ee9-151">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d5ee9-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d5ee9-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="d5ee9-152">managedDeviceId</span></span>|<span data-ttu-id="d5ee9-153">String</span><span class="sxs-lookup"><span data-stu-id="d5ee9-153">String</span></span>|<span data-ttu-id="d5ee9-154">Die verwaltete Geräte-ID.</span><span class="sxs-lookup"><span data-stu-id="d5ee9-154">The managed device ID.</span></span>|
|<span data-ttu-id="d5ee9-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="d5ee9-155">deviceName</span></span>|<span data-ttu-id="d5ee9-156">String</span><span class="sxs-lookup"><span data-stu-id="d5ee9-156">String</span></span>|<span data-ttu-id="d5ee9-157">Der Gerätename.</span><span class="sxs-lookup"><span data-stu-id="d5ee9-157">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="d5ee9-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5ee9-158">Response</span></span>
<span data-ttu-id="d5ee9-159">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d5ee9-159">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5ee9-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d5ee9-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5ee9-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5ee9-161">Request</span></span>
<span data-ttu-id="d5ee9-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d5ee9-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 327

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="d5ee9-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5ee9-163">Response</span></span>
<span data-ttu-id="d5ee9-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d5ee9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
  "id": "bed943d0-43d0-bed9-d043-d9bed043d9be",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value"
}
```




