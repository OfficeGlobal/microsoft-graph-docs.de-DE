---
title: Erstellen von iosVppAppAssignedDeviceLicense
description: Erstellen eines neuen IosVppAppAssignedDeviceLicense-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2806e6db550068f46e943f03baca96647176912a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410469"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="441e4-103">Erstellen von iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="441e4-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="441e4-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="441e4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="441e4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="441e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="441e4-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="441e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="441e4-107">Erstellen eines neuen [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="441e4-107">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="441e4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="441e4-108">Prerequisites</span></span>
<span data-ttu-id="441e4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="441e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="441e4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="441e4-111">Permission type</span></span>|<span data-ttu-id="441e4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="441e4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="441e4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="441e4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="441e4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="441e4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="441e4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="441e4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="441e4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="441e4-116">Not supported.</span></span>|
|<span data-ttu-id="441e4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="441e4-117">Application</span></span>|<span data-ttu-id="441e4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="441e4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="441e4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="441e4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="441e4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="441e4-120">Request headers</span></span>
|<span data-ttu-id="441e4-121">Header</span><span class="sxs-lookup"><span data-stu-id="441e4-121">Header</span></span>|<span data-ttu-id="441e4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="441e4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="441e4-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="441e4-123">Authorization</span></span>|<span data-ttu-id="441e4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="441e4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="441e4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="441e4-125">Accept</span></span>|<span data-ttu-id="441e4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="441e4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="441e4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="441e4-127">Request body</span></span>
<span data-ttu-id="441e4-128">Geben Sie im Textkörper Anforderung für das Objekt IosVppAppAssignedDeviceLicense eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="441e4-128">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="441e4-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die IosVppAppAssignedDeviceLicense erstellen.</span><span class="sxs-lookup"><span data-stu-id="441e4-129">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="441e4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="441e4-130">Property</span></span>|<span data-ttu-id="441e4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="441e4-131">Type</span></span>|<span data-ttu-id="441e4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="441e4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="441e4-133">id</span><span class="sxs-lookup"><span data-stu-id="441e4-133">id</span></span>|<span data-ttu-id="441e4-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="441e4-134">String</span></span>|<span data-ttu-id="441e4-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="441e4-135">Key of the entity.</span></span> <span data-ttu-id="441e4-136">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="441e4-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="441e4-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="441e4-137">userEmailAddress</span></span>|<span data-ttu-id="441e4-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="441e4-138">String</span></span>|<span data-ttu-id="441e4-139">Die e-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="441e4-139">The user email address.</span></span> <span data-ttu-id="441e4-140">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="441e4-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="441e4-141">userId</span><span class="sxs-lookup"><span data-stu-id="441e4-141">userId</span></span>|<span data-ttu-id="441e4-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="441e4-142">String</span></span>|<span data-ttu-id="441e4-143">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="441e4-143">The user ID.</span></span> <span data-ttu-id="441e4-144">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="441e4-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="441e4-145">userName</span><span class="sxs-lookup"><span data-stu-id="441e4-145">userName</span></span>|<span data-ttu-id="441e4-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="441e4-146">String</span></span>|<span data-ttu-id="441e4-147">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="441e4-147">The user name.</span></span> <span data-ttu-id="441e4-148">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="441e4-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="441e4-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="441e4-149">userPrincipalName</span></span>|<span data-ttu-id="441e4-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="441e4-150">String</span></span>|<span data-ttu-id="441e4-151">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="441e4-151">The user principal name.</span></span> <span data-ttu-id="441e4-152">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="441e4-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="441e4-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="441e4-153">managedDeviceId</span></span>|<span data-ttu-id="441e4-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="441e4-154">String</span></span>|<span data-ttu-id="441e4-155">Die verwaltete Geräte-ID.</span><span class="sxs-lookup"><span data-stu-id="441e4-155">The managed device ID.</span></span>|
|<span data-ttu-id="441e4-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="441e4-156">deviceName</span></span>|<span data-ttu-id="441e4-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="441e4-157">String</span></span>|<span data-ttu-id="441e4-158">Der Name des Aufnahmegeräts.</span><span class="sxs-lookup"><span data-stu-id="441e4-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="441e4-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="441e4-159">Response</span></span>
<span data-ttu-id="441e4-160">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="441e4-160">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="441e4-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="441e4-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="441e4-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="441e4-162">Request</span></span>
<span data-ttu-id="441e4-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="441e4-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="441e4-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="441e4-164">Response</span></span>
<span data-ttu-id="441e4-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="441e4-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




