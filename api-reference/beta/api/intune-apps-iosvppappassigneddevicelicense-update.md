---
title: IosVppAppAssignedDeviceLicense aktualisieren
description: Aktualisieren Sie die Eigenschaften eines IosVppAppAssignedDeviceLicense-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2edd886b0ab9b302e7f224511bb329fe8269a7d9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402125"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="ecf37-103">IosVppAppAssignedDeviceLicense aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ecf37-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="ecf37-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ecf37-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ecf37-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ecf37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ecf37-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ecf37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecf37-107">Aktualisieren Sie die Eigenschaften eines [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ecf37-107">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecf37-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ecf37-108">Prerequisites</span></span>
<span data-ttu-id="ecf37-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ecf37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ecf37-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ecf37-111">Permission type</span></span>|<span data-ttu-id="ecf37-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ecf37-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecf37-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ecf37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ecf37-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecf37-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ecf37-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ecf37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecf37-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ecf37-116">Not supported.</span></span>|
|<span data-ttu-id="ecf37-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ecf37-117">Application</span></span>|<span data-ttu-id="ecf37-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ecf37-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecf37-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ecf37-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="ecf37-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ecf37-120">Request headers</span></span>
|<span data-ttu-id="ecf37-121">Header</span><span class="sxs-lookup"><span data-stu-id="ecf37-121">Header</span></span>|<span data-ttu-id="ecf37-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ecf37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecf37-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ecf37-123">Authorization</span></span>|<span data-ttu-id="ecf37-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ecf37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecf37-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ecf37-125">Accept</span></span>|<span data-ttu-id="ecf37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ecf37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecf37-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ecf37-127">Request body</span></span>
<span data-ttu-id="ecf37-128">Geben Sie im Textkörper Anforderung für das Objekt [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="ecf37-128">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="ecf37-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="ecf37-129">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="ecf37-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ecf37-130">Property</span></span>|<span data-ttu-id="ecf37-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ecf37-131">Type</span></span>|<span data-ttu-id="ecf37-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ecf37-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecf37-133">id</span><span class="sxs-lookup"><span data-stu-id="ecf37-133">id</span></span>|<span data-ttu-id="ecf37-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecf37-134">String</span></span>|<span data-ttu-id="ecf37-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ecf37-135">Key of the entity.</span></span> <span data-ttu-id="ecf37-136">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="ecf37-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ecf37-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="ecf37-137">userEmailAddress</span></span>|<span data-ttu-id="ecf37-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecf37-138">String</span></span>|<span data-ttu-id="ecf37-139">Die e-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="ecf37-139">The user email address.</span></span> <span data-ttu-id="ecf37-140">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="ecf37-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ecf37-141">userId</span><span class="sxs-lookup"><span data-stu-id="ecf37-141">userId</span></span>|<span data-ttu-id="ecf37-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecf37-142">String</span></span>|<span data-ttu-id="ecf37-143">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="ecf37-143">The user ID.</span></span> <span data-ttu-id="ecf37-144">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="ecf37-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ecf37-145">userName</span><span class="sxs-lookup"><span data-stu-id="ecf37-145">userName</span></span>|<span data-ttu-id="ecf37-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecf37-146">String</span></span>|<span data-ttu-id="ecf37-147">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="ecf37-147">The user name.</span></span> <span data-ttu-id="ecf37-148">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="ecf37-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ecf37-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ecf37-149">userPrincipalName</span></span>|<span data-ttu-id="ecf37-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecf37-150">String</span></span>|<span data-ttu-id="ecf37-151">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="ecf37-151">The user principal name.</span></span> <span data-ttu-id="ecf37-152">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="ecf37-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ecf37-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="ecf37-153">managedDeviceId</span></span>|<span data-ttu-id="ecf37-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecf37-154">String</span></span>|<span data-ttu-id="ecf37-155">Die verwaltete Geräte-ID.</span><span class="sxs-lookup"><span data-stu-id="ecf37-155">The managed device ID.</span></span>|
|<span data-ttu-id="ecf37-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="ecf37-156">deviceName</span></span>|<span data-ttu-id="ecf37-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecf37-157">String</span></span>|<span data-ttu-id="ecf37-158">Der Name des Aufnahmegeräts.</span><span class="sxs-lookup"><span data-stu-id="ecf37-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="ecf37-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="ecf37-159">Response</span></span>
<span data-ttu-id="ecf37-160">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ecf37-160">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecf37-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ecf37-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecf37-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ecf37-162">Request</span></span>
<span data-ttu-id="ecf37-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ecf37-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ecf37-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="ecf37-164">Response</span></span>
<span data-ttu-id="ecf37-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ecf37-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




