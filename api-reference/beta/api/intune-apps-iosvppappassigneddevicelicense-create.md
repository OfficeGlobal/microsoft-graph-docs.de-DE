---
title: IosVppAppAssignedDeviceLicense erstellen
description: Erstellen eines neuen iosVppAppAssignedDeviceLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42109f11ffb01fa90b5ecde9e7952d4113fb23ba
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972907"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="abb82-103">IosVppAppAssignedDeviceLicense erstellen</span><span class="sxs-lookup"><span data-stu-id="abb82-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="abb82-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="abb82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abb82-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="abb82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abb82-106">Erstellen eines neuen [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="abb82-106">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abb82-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="abb82-107">Prerequisites</span></span>
<span data-ttu-id="abb82-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abb82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abb82-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="abb82-110">Permission type</span></span>|<span data-ttu-id="abb82-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="abb82-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abb82-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="abb82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abb82-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abb82-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="abb82-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="abb82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abb82-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abb82-115">Not supported.</span></span>|
|<span data-ttu-id="abb82-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="abb82-116">Application</span></span>|<span data-ttu-id="abb82-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abb82-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abb82-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="abb82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="abb82-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="abb82-119">Request headers</span></span>
|<span data-ttu-id="abb82-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="abb82-120">Header</span></span>|<span data-ttu-id="abb82-121">Wert</span><span class="sxs-lookup"><span data-stu-id="abb82-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abb82-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="abb82-122">Authorization</span></span>|<span data-ttu-id="abb82-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="abb82-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abb82-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="abb82-124">Accept</span></span>|<span data-ttu-id="abb82-125">application/json</span><span class="sxs-lookup"><span data-stu-id="abb82-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abb82-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="abb82-126">Request body</span></span>
<span data-ttu-id="abb82-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das iosVppAppAssignedDeviceLicense-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="abb82-127">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="abb82-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosVppAppAssignedDeviceLicense erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="abb82-128">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="abb82-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="abb82-129">Property</span></span>|<span data-ttu-id="abb82-130">Typ</span><span class="sxs-lookup"><span data-stu-id="abb82-130">Type</span></span>|<span data-ttu-id="abb82-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="abb82-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abb82-132">id</span><span class="sxs-lookup"><span data-stu-id="abb82-132">id</span></span>|<span data-ttu-id="abb82-133">String</span><span class="sxs-lookup"><span data-stu-id="abb82-133">String</span></span>|<span data-ttu-id="abb82-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="abb82-134">Key of the entity.</span></span> <span data-ttu-id="abb82-135">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="abb82-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="abb82-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="abb82-136">userEmailAddress</span></span>|<span data-ttu-id="abb82-137">String</span><span class="sxs-lookup"><span data-stu-id="abb82-137">String</span></span>|<span data-ttu-id="abb82-138">Die Benutzer-e-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="abb82-138">The user email address.</span></span> <span data-ttu-id="abb82-139">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="abb82-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="abb82-140">userId</span><span class="sxs-lookup"><span data-stu-id="abb82-140">userId</span></span>|<span data-ttu-id="abb82-141">String</span><span class="sxs-lookup"><span data-stu-id="abb82-141">String</span></span>|<span data-ttu-id="abb82-142">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="abb82-142">The user ID.</span></span> <span data-ttu-id="abb82-143">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="abb82-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="abb82-144">userName</span><span class="sxs-lookup"><span data-stu-id="abb82-144">userName</span></span>|<span data-ttu-id="abb82-145">String</span><span class="sxs-lookup"><span data-stu-id="abb82-145">String</span></span>|<span data-ttu-id="abb82-146">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="abb82-146">The user name.</span></span> <span data-ttu-id="abb82-147">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="abb82-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="abb82-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="abb82-148">userPrincipalName</span></span>|<span data-ttu-id="abb82-149">String</span><span class="sxs-lookup"><span data-stu-id="abb82-149">String</span></span>|<span data-ttu-id="abb82-150">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="abb82-150">The user principal name.</span></span> <span data-ttu-id="abb82-151">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="abb82-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="abb82-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="abb82-152">managedDeviceId</span></span>|<span data-ttu-id="abb82-153">String</span><span class="sxs-lookup"><span data-stu-id="abb82-153">String</span></span>|<span data-ttu-id="abb82-154">Die verwaltete Geräte-ID.</span><span class="sxs-lookup"><span data-stu-id="abb82-154">The managed device ID.</span></span>|
|<span data-ttu-id="abb82-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="abb82-155">deviceName</span></span>|<span data-ttu-id="abb82-156">String</span><span class="sxs-lookup"><span data-stu-id="abb82-156">String</span></span>|<span data-ttu-id="abb82-157">Der Gerätename.</span><span class="sxs-lookup"><span data-stu-id="abb82-157">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="abb82-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="abb82-158">Response</span></span>
<span data-ttu-id="abb82-159">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="abb82-159">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abb82-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="abb82-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="abb82-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="abb82-161">Request</span></span>
<span data-ttu-id="abb82-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="abb82-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
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

### <a name="response"></a><span data-ttu-id="abb82-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="abb82-163">Response</span></span>
<span data-ttu-id="abb82-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="abb82-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




