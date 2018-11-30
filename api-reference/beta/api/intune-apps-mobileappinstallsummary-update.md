---
title: MobileAppInstallSummary aktualisieren
description: Aktualisieren Sie die Eigenschaften eines MobileAppInstallSummary-Objekts.
ms.openlocfilehash: 0fa1343d52fa82c69f6511d3e320ebae2d98a084
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059901"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="71401-103">MobileAppInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="71401-103">Update mobileAppInstallSummary</span></span>

> <span data-ttu-id="71401-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="71401-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71401-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="71401-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71401-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="71401-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71401-107">Aktualisieren Sie die Eigenschaften eines [MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="71401-107">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71401-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="71401-108">Prerequisites</span></span>
<span data-ttu-id="71401-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71401-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71401-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71401-111">Permission type</span></span>|<span data-ttu-id="71401-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71401-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71401-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71401-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71401-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71401-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="71401-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71401-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71401-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71401-116">Not supported.</span></span>|
|<span data-ttu-id="71401-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71401-117">Application</span></span>|<span data-ttu-id="71401-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71401-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71401-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71401-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="71401-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71401-120">Request headers</span></span>
|<span data-ttu-id="71401-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="71401-121">Header</span></span>|<span data-ttu-id="71401-122">Wert</span><span class="sxs-lookup"><span data-stu-id="71401-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71401-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71401-123">Authorization</span></span>|<span data-ttu-id="71401-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="71401-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71401-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71401-125">Accept</span></span>|<span data-ttu-id="71401-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71401-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71401-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71401-127">Request body</span></span>
<span data-ttu-id="71401-128">Geben Sie im Textkörper Anforderung für das Objekt [MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="71401-128">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="71401-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="71401-129">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="71401-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71401-130">Property</span></span>|<span data-ttu-id="71401-131">Typ</span><span class="sxs-lookup"><span data-stu-id="71401-131">Type</span></span>|<span data-ttu-id="71401-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71401-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71401-133">id</span><span class="sxs-lookup"><span data-stu-id="71401-133">id</span></span>|<span data-ttu-id="71401-134">String</span><span class="sxs-lookup"><span data-stu-id="71401-134">String</span></span>|<span data-ttu-id="71401-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="71401-135">Key of the entity.</span></span>|
|<span data-ttu-id="71401-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="71401-136">installedDeviceCount</span></span>|<span data-ttu-id="71401-137">Int32</span><span class="sxs-lookup"><span data-stu-id="71401-137">Int32</span></span>|<span data-ttu-id="71401-138">Anzahl der Geräte, die diese app erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="71401-138">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="71401-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="71401-139">failedDeviceCount</span></span>|<span data-ttu-id="71401-140">Int32</span><span class="sxs-lookup"><span data-stu-id="71401-140">Int32</span></span>|<span data-ttu-id="71401-141">Anzahl der Geräte, die fehlgeschlagen sind, um diese app zu installieren.</span><span class="sxs-lookup"><span data-stu-id="71401-141">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="71401-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="71401-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="71401-143">Int32</span><span class="sxs-lookup"><span data-stu-id="71401-143">Int32</span></span>|<span data-ttu-id="71401-144">Anzahl der Geräte, die für diese app nicht zutreffen.</span><span class="sxs-lookup"><span data-stu-id="71401-144">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="71401-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="71401-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="71401-146">Int32</span><span class="sxs-lookup"><span data-stu-id="71401-146">Int32</span></span>|<span data-ttu-id="71401-147">Anzahl der Geräte, die diese app installiert nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="71401-147">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="71401-148">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="71401-148">pendingInstallDeviceCount</span></span>|<span data-ttu-id="71401-149">Int32</span><span class="sxs-lookup"><span data-stu-id="71401-149">Int32</span></span>|<span data-ttu-id="71401-150">Anzahl der Geräte, die diese app installieren benachrichtigt wurden.</span><span class="sxs-lookup"><span data-stu-id="71401-150">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="71401-151">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="71401-151">installedUserCount</span></span>|<span data-ttu-id="71401-152">Int32</span><span class="sxs-lookup"><span data-stu-id="71401-152">Int32</span></span>|<span data-ttu-id="71401-153">Anzahl der Benutzer, deren Geräte alle erfolgreich ausgeführt wurden, um diese app zu installieren.</span><span class="sxs-lookup"><span data-stu-id="71401-153">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="71401-154">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="71401-154">failedUserCount</span></span>|<span data-ttu-id="71401-155">Int32</span><span class="sxs-lookup"><span data-stu-id="71401-155">Int32</span></span>|<span data-ttu-id="71401-156">Anzahl der Benutzer, die 1 haben oder weitere Gerät, deren Installation diese app fehlschlug.</span><span class="sxs-lookup"><span data-stu-id="71401-156">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="71401-157">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="71401-157">notApplicableUserCount</span></span>|<span data-ttu-id="71401-158">Int32</span><span class="sxs-lookup"><span data-stu-id="71401-158">Int32</span></span>|<span data-ttu-id="71401-159">Anzahl der Benutzer, deren Geräte alle nicht zutreffend für diese app waren.</span><span class="sxs-lookup"><span data-stu-id="71401-159">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="71401-160">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="71401-160">notInstalledUserCount</span></span>|<span data-ttu-id="71401-161">Int32</span><span class="sxs-lookup"><span data-stu-id="71401-161">Int32</span></span>|<span data-ttu-id="71401-162">Anzahl der Benutzer mit 1 oder mehrere Geräte, die diese app nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="71401-162">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="71401-163">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="71401-163">pendingInstallUserCount</span></span>|<span data-ttu-id="71401-164">Int32</span><span class="sxs-lookup"><span data-stu-id="71401-164">Int32</span></span>|<span data-ttu-id="71401-165">Anzahl der Benutzer, die 1 haben oder weitere Geräte, die diese app installieren und 0 Geräte mit Fehlern benachrichtigt wurden.</span><span class="sxs-lookup"><span data-stu-id="71401-165">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="71401-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="71401-166">Response</span></span>
<span data-ttu-id="71401-167">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="71401-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71401-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71401-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="71401-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71401-169">Request</span></span>
<span data-ttu-id="71401-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71401-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 312

{
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

### <a name="response"></a><span data-ttu-id="71401-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="71401-171">Response</span></span>
<span data-ttu-id="71401-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71401-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





