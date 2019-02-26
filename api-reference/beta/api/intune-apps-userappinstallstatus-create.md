---
title: UserAppInstallStatus erstellen
description: Erstellen eines neuen userAppInstallStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8028aadae940fe9ff792b5e403f737727b2d5399
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172072"
---
# <a name="create-userappinstallstatus"></a><span data-ttu-id="b2b60-103">UserAppInstallStatus erstellen</span><span class="sxs-lookup"><span data-stu-id="b2b60-103">Create userAppInstallStatus</span></span>

> <span data-ttu-id="b2b60-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b2b60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2b60-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b2b60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2b60-106">Erstellen eines neuen [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b2b60-106">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2b60-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b2b60-107">Prerequisites</span></span>
<span data-ttu-id="b2b60-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b2b60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b2b60-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b2b60-110">Permission type</span></span>|<span data-ttu-id="b2b60-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b2b60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2b60-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b2b60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2b60-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2b60-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b2b60-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b2b60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2b60-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b2b60-115">Not supported.</span></span>|
|<span data-ttu-id="b2b60-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b2b60-116">Application</span></span>|<span data-ttu-id="b2b60-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b2b60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2b60-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2b60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b2b60-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b2b60-119">Request headers</span></span>
|<span data-ttu-id="b2b60-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b2b60-120">Header</span></span>|<span data-ttu-id="b2b60-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b2b60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2b60-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2b60-122">Authorization</span></span>|<span data-ttu-id="b2b60-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b2b60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2b60-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b2b60-124">Accept</span></span>|<span data-ttu-id="b2b60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2b60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2b60-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b2b60-126">Request body</span></span>
<span data-ttu-id="b2b60-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das userAppInstallStatus-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b2b60-127">In the request body, supply a JSON representation for the userAppInstallStatus object.</span></span>

<span data-ttu-id="b2b60-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der userAppInstallStatus erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b2b60-128">The following table shows the properties that are required when you create the userAppInstallStatus.</span></span>

|<span data-ttu-id="b2b60-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b2b60-129">Property</span></span>|<span data-ttu-id="b2b60-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b2b60-130">Type</span></span>|<span data-ttu-id="b2b60-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2b60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2b60-132">id</span><span class="sxs-lookup"><span data-stu-id="b2b60-132">id</span></span>|<span data-ttu-id="b2b60-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2b60-133">String</span></span>|<span data-ttu-id="b2b60-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b2b60-134">Key of the entity.</span></span>|
|<span data-ttu-id="b2b60-135">userName</span><span class="sxs-lookup"><span data-stu-id="b2b60-135">userName</span></span>|<span data-ttu-id="b2b60-136">String</span><span class="sxs-lookup"><span data-stu-id="b2b60-136">String</span></span>|<span data-ttu-id="b2b60-137">Name des Benutzers</span><span class="sxs-lookup"><span data-stu-id="b2b60-137">User name.</span></span>|
|<span data-ttu-id="b2b60-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b2b60-138">userPrincipalName</span></span>|<span data-ttu-id="b2b60-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2b60-139">String</span></span>|<span data-ttu-id="b2b60-140">Benutzerprinzipal Name.</span><span class="sxs-lookup"><span data-stu-id="b2b60-140">User Principal Name.</span></span>|
|<span data-ttu-id="b2b60-141">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b2b60-141">installedDeviceCount</span></span>|<span data-ttu-id="b2b60-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b2b60-142">Int32</span></span>|<span data-ttu-id="b2b60-143">Anzahl der installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="b2b60-143">Installed Device Count.</span></span>|
|<span data-ttu-id="b2b60-144">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b2b60-144">failedDeviceCount</span></span>|<span data-ttu-id="b2b60-145">Int32</span><span class="sxs-lookup"><span data-stu-id="b2b60-145">Int32</span></span>|<span data-ttu-id="b2b60-146">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="b2b60-146">Failed Device Count.</span></span>|
|<span data-ttu-id="b2b60-147">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b2b60-147">notInstalledDeviceCount</span></span>|<span data-ttu-id="b2b60-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b2b60-148">Int32</span></span>|<span data-ttu-id="b2b60-149">Anzahl der nicht installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="b2b60-149">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="b2b60-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2b60-150">Response</span></span>
<span data-ttu-id="b2b60-151">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b2b60-151">If successful, this method returns a `201 Created` response code and a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2b60-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b2b60-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2b60-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2b60-153">Request</span></span>
<span data-ttu-id="b2b60-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b2b60-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="b2b60-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2b60-155">Response</span></span>
<span data-ttu-id="b2b60-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b2b60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




