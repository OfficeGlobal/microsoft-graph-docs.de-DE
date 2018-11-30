---
title: IosVppAppAssignedDeviceLicense aktualisieren
description: Aktualisieren Sie die Eigenschaften eines IosVppAppAssignedDeviceLicense-Objekts.
ms.openlocfilehash: 8e2d623dd1d5c3b1f69fb62244a8eb20af3b3f95
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059257"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="64897-103">IosVppAppAssignedDeviceLicense aktualisieren</span><span class="sxs-lookup"><span data-stu-id="64897-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="64897-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="64897-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64897-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="64897-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64897-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="64897-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64897-107">Aktualisieren Sie die Eigenschaften eines [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="64897-107">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="64897-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="64897-108">Prerequisites</span></span>
<span data-ttu-id="64897-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64897-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64897-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="64897-111">Permission type</span></span>|<span data-ttu-id="64897-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="64897-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64897-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="64897-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64897-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64897-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="64897-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="64897-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64897-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64897-116">Not supported.</span></span>|
|<span data-ttu-id="64897-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="64897-117">Application</span></span>|<span data-ttu-id="64897-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64897-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64897-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="64897-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="64897-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="64897-120">Request headers</span></span>
|<span data-ttu-id="64897-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="64897-121">Header</span></span>|<span data-ttu-id="64897-122">Wert</span><span class="sxs-lookup"><span data-stu-id="64897-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64897-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64897-123">Authorization</span></span>|<span data-ttu-id="64897-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="64897-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64897-125">Accept</span><span class="sxs-lookup"><span data-stu-id="64897-125">Accept</span></span>|<span data-ttu-id="64897-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64897-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64897-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="64897-127">Request body</span></span>
<span data-ttu-id="64897-128">Geben Sie im Textkörper Anforderung für das Objekt [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="64897-128">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="64897-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="64897-129">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="64897-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="64897-130">Property</span></span>|<span data-ttu-id="64897-131">Typ</span><span class="sxs-lookup"><span data-stu-id="64897-131">Type</span></span>|<span data-ttu-id="64897-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64897-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64897-133">id</span><span class="sxs-lookup"><span data-stu-id="64897-133">id</span></span>|<span data-ttu-id="64897-134">String</span><span class="sxs-lookup"><span data-stu-id="64897-134">String</span></span>|<span data-ttu-id="64897-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="64897-135">Key of the entity.</span></span> <span data-ttu-id="64897-136">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="64897-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="64897-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="64897-137">userEmailAddress</span></span>|<span data-ttu-id="64897-138">String</span><span class="sxs-lookup"><span data-stu-id="64897-138">String</span></span>|<span data-ttu-id="64897-139">Die e-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="64897-139">The user email address.</span></span> <span data-ttu-id="64897-140">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="64897-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="64897-141">userId</span><span class="sxs-lookup"><span data-stu-id="64897-141">userId</span></span>|<span data-ttu-id="64897-142">String</span><span class="sxs-lookup"><span data-stu-id="64897-142">String</span></span>|<span data-ttu-id="64897-143">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="64897-143">The user ID.</span></span> <span data-ttu-id="64897-144">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="64897-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="64897-145">userName</span><span class="sxs-lookup"><span data-stu-id="64897-145">userName</span></span>|<span data-ttu-id="64897-146">String</span><span class="sxs-lookup"><span data-stu-id="64897-146">String</span></span>|<span data-ttu-id="64897-147">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="64897-147">The user name.</span></span> <span data-ttu-id="64897-148">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="64897-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="64897-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="64897-149">userPrincipalName</span></span>|<span data-ttu-id="64897-150">String</span><span class="sxs-lookup"><span data-stu-id="64897-150">String</span></span>|<span data-ttu-id="64897-151">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="64897-151">The user principal name.</span></span> <span data-ttu-id="64897-152">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="64897-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="64897-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="64897-153">managedDeviceId</span></span>|<span data-ttu-id="64897-154">String</span><span class="sxs-lookup"><span data-stu-id="64897-154">String</span></span>|<span data-ttu-id="64897-155">Die verwaltete Geräte-ID.</span><span class="sxs-lookup"><span data-stu-id="64897-155">The managed device ID.</span></span>|
|<span data-ttu-id="64897-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="64897-156">deviceName</span></span>|<span data-ttu-id="64897-157">String</span><span class="sxs-lookup"><span data-stu-id="64897-157">String</span></span>|<span data-ttu-id="64897-158">Der Name des Aufnahmegeräts.</span><span class="sxs-lookup"><span data-stu-id="64897-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="64897-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="64897-159">Response</span></span>
<span data-ttu-id="64897-160">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="64897-160">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64897-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="64897-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="64897-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="64897-162">Request</span></span>
<span data-ttu-id="64897-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="64897-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 258

{
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="64897-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="64897-164">Response</span></span>
<span data-ttu-id="64897-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64897-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





