---
title: MobileAppInstallSummary aktualisieren
description: Aktualisieren der Eigenschaften eines mobileAppInstallSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 980f6b9c4712bea8fd4060f627603310ef8c6747
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959663"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="111cc-103">MobileAppInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="111cc-103">Update mobileAppInstallSummary</span></span>

> <span data-ttu-id="111cc-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="111cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="111cc-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="111cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="111cc-106">Aktualisieren der Eigenschaften eines [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="111cc-106">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="111cc-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="111cc-107">Prerequisites</span></span>
<span data-ttu-id="111cc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="111cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="111cc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="111cc-110">Permission type</span></span>|<span data-ttu-id="111cc-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="111cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="111cc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="111cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="111cc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="111cc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="111cc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="111cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="111cc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="111cc-115">Not supported.</span></span>|
|<span data-ttu-id="111cc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="111cc-116">Application</span></span>|<span data-ttu-id="111cc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="111cc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="111cc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="111cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="111cc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="111cc-119">Request headers</span></span>
|<span data-ttu-id="111cc-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="111cc-120">Header</span></span>|<span data-ttu-id="111cc-121">Wert</span><span class="sxs-lookup"><span data-stu-id="111cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="111cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="111cc-122">Authorization</span></span>|<span data-ttu-id="111cc-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="111cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="111cc-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="111cc-124">Accept</span></span>|<span data-ttu-id="111cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="111cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="111cc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="111cc-126">Request body</span></span>
<span data-ttu-id="111cc-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="111cc-127">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="111cc-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="111cc-128">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="111cc-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="111cc-129">Property</span></span>|<span data-ttu-id="111cc-130">Typ</span><span class="sxs-lookup"><span data-stu-id="111cc-130">Type</span></span>|<span data-ttu-id="111cc-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="111cc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="111cc-132">id</span><span class="sxs-lookup"><span data-stu-id="111cc-132">id</span></span>|<span data-ttu-id="111cc-133">String</span><span class="sxs-lookup"><span data-stu-id="111cc-133">String</span></span>|<span data-ttu-id="111cc-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="111cc-134">Key of the entity.</span></span>|
|<span data-ttu-id="111cc-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="111cc-135">installedDeviceCount</span></span>|<span data-ttu-id="111cc-136">Int32</span><span class="sxs-lookup"><span data-stu-id="111cc-136">Int32</span></span>|<span data-ttu-id="111cc-137">Die Anzahl der Geräte, die diese APP erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="111cc-137">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="111cc-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="111cc-138">failedDeviceCount</span></span>|<span data-ttu-id="111cc-139">Int32</span><span class="sxs-lookup"><span data-stu-id="111cc-139">Int32</span></span>|<span data-ttu-id="111cc-140">Anzahl der Geräte, die diese APP nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="111cc-140">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="111cc-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="111cc-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="111cc-142">Int32</span><span class="sxs-lookup"><span data-stu-id="111cc-142">Int32</span></span>|<span data-ttu-id="111cc-143">Die Anzahl der Geräte, die für diese APP nicht anwendbar sind.</span><span class="sxs-lookup"><span data-stu-id="111cc-143">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="111cc-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="111cc-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="111cc-145">Int32</span><span class="sxs-lookup"><span data-stu-id="111cc-145">Int32</span></span>|<span data-ttu-id="111cc-146">Anzahl der Geräte, auf denen diese APP nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="111cc-146">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="111cc-147">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="111cc-147">pendingInstallDeviceCount</span></span>|<span data-ttu-id="111cc-148">Int32</span><span class="sxs-lookup"><span data-stu-id="111cc-148">Int32</span></span>|<span data-ttu-id="111cc-149">Anzahl der Geräte, die zur Installation dieser APP benachrichtigt wurden.</span><span class="sxs-lookup"><span data-stu-id="111cc-149">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="111cc-150">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="111cc-150">installedUserCount</span></span>|<span data-ttu-id="111cc-151">Int32</span><span class="sxs-lookup"><span data-stu-id="111cc-151">Int32</span></span>|<span data-ttu-id="111cc-152">Die Anzahl der Benutzer, deren Geräte alle für die Installation dieser APP erfolgreich waren.</span><span class="sxs-lookup"><span data-stu-id="111cc-152">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="111cc-153">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="111cc-153">failedUserCount</span></span>|<span data-ttu-id="111cc-154">Int32</span><span class="sxs-lookup"><span data-stu-id="111cc-154">Int32</span></span>|<span data-ttu-id="111cc-155">Die Anzahl der Benutzer, die über ein Gerät verfügen, für das diese APP nicht installiert werden konnte.</span><span class="sxs-lookup"><span data-stu-id="111cc-155">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="111cc-156">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="111cc-156">notApplicableUserCount</span></span>|<span data-ttu-id="111cc-157">Int32</span><span class="sxs-lookup"><span data-stu-id="111cc-157">Int32</span></span>|<span data-ttu-id="111cc-158">Die Anzahl der Benutzer, deren Geräte für diese APP nicht anwendbar waren.</span><span class="sxs-lookup"><span data-stu-id="111cc-158">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="111cc-159">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="111cc-159">notInstalledUserCount</span></span>|<span data-ttu-id="111cc-160">Int32</span><span class="sxs-lookup"><span data-stu-id="111cc-160">Int32</span></span>|<span data-ttu-id="111cc-161">Die Anzahl von Benutzern, die über 1 oder mehr Geräte verfügen, die diese APP nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="111cc-161">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="111cc-162">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="111cc-162">pendingInstallUserCount</span></span>|<span data-ttu-id="111cc-163">Int32</span><span class="sxs-lookup"><span data-stu-id="111cc-163">Int32</span></span>|<span data-ttu-id="111cc-164">Die Anzahl der Benutzer mit mindestens 1 Gerät, die zur Installation dieser APP benachrichtigt wurden und über 0 Geräte mit Fehlern verfügen.</span><span class="sxs-lookup"><span data-stu-id="111cc-164">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="111cc-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="111cc-165">Response</span></span>
<span data-ttu-id="111cc-166">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="111cc-166">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="111cc-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="111cc-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="111cc-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="111cc-168">Request</span></span>
<span data-ttu-id="111cc-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="111cc-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```

### <a name="response"></a><span data-ttu-id="111cc-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="111cc-170">Response</span></span>
<span data-ttu-id="111cc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="111cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "06a792e9-92e9-06a7-e992-a706e992a706",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```




