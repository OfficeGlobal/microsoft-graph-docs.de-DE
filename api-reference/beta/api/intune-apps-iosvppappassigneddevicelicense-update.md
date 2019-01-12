---
title: IosVppAppAssignedDeviceLicense aktualisieren
description: Aktualisieren Sie die Eigenschaften eines IosVppAppAssignedDeviceLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b8f18e1fb8895861cd497204f9b9608f7c4f9dba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974182"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="16af6-103">IosVppAppAssignedDeviceLicense aktualisieren</span><span class="sxs-lookup"><span data-stu-id="16af6-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="16af6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="16af6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16af6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16af6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16af6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="16af6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16af6-107">Aktualisieren Sie die Eigenschaften eines [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="16af6-107">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16af6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="16af6-108">Prerequisites</span></span>
<span data-ttu-id="16af6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16af6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16af6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="16af6-111">Permission type</span></span>|<span data-ttu-id="16af6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="16af6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16af6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="16af6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16af6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16af6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="16af6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="16af6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16af6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16af6-116">Not supported.</span></span>|
|<span data-ttu-id="16af6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="16af6-117">Application</span></span>|<span data-ttu-id="16af6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16af6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16af6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="16af6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="16af6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="16af6-120">Request headers</span></span>
|<span data-ttu-id="16af6-121">Header</span><span class="sxs-lookup"><span data-stu-id="16af6-121">Header</span></span>|<span data-ttu-id="16af6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="16af6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16af6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16af6-123">Authorization</span></span>|<span data-ttu-id="16af6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="16af6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16af6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="16af6-125">Accept</span></span>|<span data-ttu-id="16af6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16af6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16af6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="16af6-127">Request body</span></span>
<span data-ttu-id="16af6-128">Geben Sie im Textkörper Anforderung für das Objekt [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="16af6-128">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="16af6-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="16af6-129">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="16af6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16af6-130">Property</span></span>|<span data-ttu-id="16af6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="16af6-131">Type</span></span>|<span data-ttu-id="16af6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16af6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16af6-133">id</span><span class="sxs-lookup"><span data-stu-id="16af6-133">id</span></span>|<span data-ttu-id="16af6-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="16af6-134">String</span></span>|<span data-ttu-id="16af6-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="16af6-135">Key of the entity.</span></span> <span data-ttu-id="16af6-136">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="16af6-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="16af6-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="16af6-137">userEmailAddress</span></span>|<span data-ttu-id="16af6-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="16af6-138">String</span></span>|<span data-ttu-id="16af6-139">Die e-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="16af6-139">The user email address.</span></span> <span data-ttu-id="16af6-140">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="16af6-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="16af6-141">userId</span><span class="sxs-lookup"><span data-stu-id="16af6-141">userId</span></span>|<span data-ttu-id="16af6-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="16af6-142">String</span></span>|<span data-ttu-id="16af6-143">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="16af6-143">The user ID.</span></span> <span data-ttu-id="16af6-144">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="16af6-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="16af6-145">userName</span><span class="sxs-lookup"><span data-stu-id="16af6-145">userName</span></span>|<span data-ttu-id="16af6-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="16af6-146">String</span></span>|<span data-ttu-id="16af6-147">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="16af6-147">The user name.</span></span> <span data-ttu-id="16af6-148">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="16af6-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="16af6-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="16af6-149">userPrincipalName</span></span>|<span data-ttu-id="16af6-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="16af6-150">String</span></span>|<span data-ttu-id="16af6-151">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="16af6-151">The user principal name.</span></span> <span data-ttu-id="16af6-152">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="16af6-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="16af6-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="16af6-153">managedDeviceId</span></span>|<span data-ttu-id="16af6-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="16af6-154">String</span></span>|<span data-ttu-id="16af6-155">Die verwaltete Geräte-ID.</span><span class="sxs-lookup"><span data-stu-id="16af6-155">The managed device ID.</span></span>|
|<span data-ttu-id="16af6-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="16af6-156">deviceName</span></span>|<span data-ttu-id="16af6-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="16af6-157">String</span></span>|<span data-ttu-id="16af6-158">Der Name des Aufnahmegeräts.</span><span class="sxs-lookup"><span data-stu-id="16af6-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="16af6-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="16af6-159">Response</span></span>
<span data-ttu-id="16af6-160">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="16af6-160">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16af6-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="16af6-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="16af6-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="16af6-162">Request</span></span>
<span data-ttu-id="16af6-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="16af6-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16af6-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="16af6-164">Response</span></span>
<span data-ttu-id="16af6-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="16af6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





