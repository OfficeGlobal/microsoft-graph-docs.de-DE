---
title: Erstellen von iosVppAppAssignedDeviceLicense
description: Erstellen eines neuen IosVppAppAssignedDeviceLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c4eecadae91eb857a5b90c88d66af1721f268ddb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914381"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="8d0e1-103">Erstellen von iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="8d0e1-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="8d0e1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d0e1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d0e1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d0e1-107">Erstellen eines neuen [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-107">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d0e1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8d0e1-108">Prerequisites</span></span>
<span data-ttu-id="8d0e1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d0e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d0e1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d0e1-111">Permission type</span></span>|<span data-ttu-id="8d0e1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d0e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d0e1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d0e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d0e1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d0e1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8d0e1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d0e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d0e1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d0e1-116">Not supported.</span></span>|
|<span data-ttu-id="8d0e1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d0e1-117">Application</span></span>|<span data-ttu-id="8d0e1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d0e1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d0e1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d0e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="8d0e1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d0e1-120">Request headers</span></span>
|<span data-ttu-id="8d0e1-121">Header</span><span class="sxs-lookup"><span data-stu-id="8d0e1-121">Header</span></span>|<span data-ttu-id="8d0e1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8d0e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d0e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d0e1-123">Authorization</span></span>|<span data-ttu-id="8d0e1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8d0e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d0e1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8d0e1-125">Accept</span></span>|<span data-ttu-id="8d0e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d0e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d0e1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d0e1-127">Request body</span></span>
<span data-ttu-id="8d0e1-128">Geben Sie im Textkörper Anforderung für das Objekt IosVppAppAssignedDeviceLicense eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-128">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="8d0e1-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die IosVppAppAssignedDeviceLicense erstellen.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-129">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="8d0e1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8d0e1-130">Property</span></span>|<span data-ttu-id="8d0e1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8d0e1-131">Type</span></span>|<span data-ttu-id="8d0e1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d0e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d0e1-133">id</span><span class="sxs-lookup"><span data-stu-id="8d0e1-133">id</span></span>|<span data-ttu-id="8d0e1-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d0e1-134">String</span></span>|<span data-ttu-id="8d0e1-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8d0e1-135">Key of the entity.</span></span> <span data-ttu-id="8d0e1-136">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8d0e1-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8d0e1-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="8d0e1-137">userEmailAddress</span></span>|<span data-ttu-id="8d0e1-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d0e1-138">String</span></span>|<span data-ttu-id="8d0e1-139">Die e-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-139">The user email address.</span></span> <span data-ttu-id="8d0e1-140">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8d0e1-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8d0e1-141">userId</span><span class="sxs-lookup"><span data-stu-id="8d0e1-141">userId</span></span>|<span data-ttu-id="8d0e1-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d0e1-142">String</span></span>|<span data-ttu-id="8d0e1-143">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-143">The user ID.</span></span> <span data-ttu-id="8d0e1-144">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8d0e1-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8d0e1-145">userName</span><span class="sxs-lookup"><span data-stu-id="8d0e1-145">userName</span></span>|<span data-ttu-id="8d0e1-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d0e1-146">String</span></span>|<span data-ttu-id="8d0e1-147">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-147">The user name.</span></span> <span data-ttu-id="8d0e1-148">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8d0e1-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8d0e1-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8d0e1-149">userPrincipalName</span></span>|<span data-ttu-id="8d0e1-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d0e1-150">String</span></span>|<span data-ttu-id="8d0e1-151">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-151">The user principal name.</span></span> <span data-ttu-id="8d0e1-152">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8d0e1-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8d0e1-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="8d0e1-153">managedDeviceId</span></span>|<span data-ttu-id="8d0e1-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d0e1-154">String</span></span>|<span data-ttu-id="8d0e1-155">Die verwaltete Geräte-ID.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-155">The managed device ID.</span></span>|
|<span data-ttu-id="8d0e1-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="8d0e1-156">deviceName</span></span>|<span data-ttu-id="8d0e1-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d0e1-157">String</span></span>|<span data-ttu-id="8d0e1-158">Der Name des Aufnahmegeräts.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="8d0e1-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d0e1-159">Response</span></span>
<span data-ttu-id="8d0e1-160">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-160">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d0e1-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d0e1-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d0e1-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d0e1-162">Request</span></span>
<span data-ttu-id="8d0e1-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8d0e1-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d0e1-164">Response</span></span>
<span data-ttu-id="8d0e1-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





