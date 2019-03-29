---
title: UserAppInstallStatus aktualisieren
description: Aktualisieren der Eigenschaften eines userAppInstallStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dce7bcd1e1c806c8f50aa6f4674104fd8d0e781b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966628"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="2ea24-103">UserAppInstallStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2ea24-103">Update userAppInstallStatus</span></span>

> <span data-ttu-id="2ea24-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2ea24-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ea24-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2ea24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ea24-106">Aktualisieren der Eigenschaften eines [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2ea24-106">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ea24-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2ea24-107">Prerequisites</span></span>
<span data-ttu-id="2ea24-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ea24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ea24-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2ea24-110">Permission type</span></span>|<span data-ttu-id="2ea24-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2ea24-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ea24-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2ea24-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ea24-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ea24-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2ea24-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2ea24-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ea24-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ea24-115">Not supported.</span></span>|
|<span data-ttu-id="2ea24-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2ea24-116">Application</span></span>|<span data-ttu-id="2ea24-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ea24-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ea24-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ea24-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="2ea24-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2ea24-119">Request headers</span></span>
|<span data-ttu-id="2ea24-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2ea24-120">Header</span></span>|<span data-ttu-id="2ea24-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2ea24-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ea24-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ea24-122">Authorization</span></span>|<span data-ttu-id="2ea24-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2ea24-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ea24-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2ea24-124">Accept</span></span>|<span data-ttu-id="2ea24-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ea24-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ea24-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2ea24-126">Request body</span></span>
<span data-ttu-id="2ea24-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="2ea24-127">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="2ea24-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2ea24-128">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="2ea24-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2ea24-129">Property</span></span>|<span data-ttu-id="2ea24-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2ea24-130">Type</span></span>|<span data-ttu-id="2ea24-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ea24-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ea24-132">id</span><span class="sxs-lookup"><span data-stu-id="2ea24-132">id</span></span>|<span data-ttu-id="2ea24-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2ea24-133">String</span></span>|<span data-ttu-id="2ea24-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2ea24-134">Key of the entity.</span></span>|
|<span data-ttu-id="2ea24-135">userName</span><span class="sxs-lookup"><span data-stu-id="2ea24-135">userName</span></span>|<span data-ttu-id="2ea24-136">String</span><span class="sxs-lookup"><span data-stu-id="2ea24-136">String</span></span>|<span data-ttu-id="2ea24-137">Name des Benutzers</span><span class="sxs-lookup"><span data-stu-id="2ea24-137">User name.</span></span>|
|<span data-ttu-id="2ea24-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2ea24-138">userPrincipalName</span></span>|<span data-ttu-id="2ea24-139">String</span><span class="sxs-lookup"><span data-stu-id="2ea24-139">String</span></span>|<span data-ttu-id="2ea24-140">Benutzerprinzipal Name.</span><span class="sxs-lookup"><span data-stu-id="2ea24-140">User Principal Name.</span></span>|
|<span data-ttu-id="2ea24-141">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ea24-141">installedDeviceCount</span></span>|<span data-ttu-id="2ea24-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2ea24-142">Int32</span></span>|<span data-ttu-id="2ea24-143">Anzahl der installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="2ea24-143">Installed Device Count.</span></span>|
|<span data-ttu-id="2ea24-144">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ea24-144">failedDeviceCount</span></span>|<span data-ttu-id="2ea24-145">Int32</span><span class="sxs-lookup"><span data-stu-id="2ea24-145">Int32</span></span>|<span data-ttu-id="2ea24-146">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="2ea24-146">Failed Device Count.</span></span>|
|<span data-ttu-id="2ea24-147">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ea24-147">notInstalledDeviceCount</span></span>|<span data-ttu-id="2ea24-148">Int32</span><span class="sxs-lookup"><span data-stu-id="2ea24-148">Int32</span></span>|<span data-ttu-id="2ea24-149">Anzahl der nicht installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="2ea24-149">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="2ea24-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ea24-150">Response</span></span>
<span data-ttu-id="2ea24-151">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2ea24-151">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ea24-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2ea24-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ea24-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ea24-153">Request</span></span>
<span data-ttu-id="2ea24-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2ea24-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
Content-type: application/json
Content-length: 239

{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="2ea24-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ea24-155">Response</span></span>
<span data-ttu-id="2ea24-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2ea24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "14959a2a-9a2a-1495-2a9a-95142a9a9514",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```




