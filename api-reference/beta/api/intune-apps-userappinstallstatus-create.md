---
title: Erstellen von userAppInstallStatus
description: Erstellen eines neuen UserAppInstallStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac22969b04f2c9191e521a3df8a51bc2d0cc3343
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985228"
---
# <a name="create-userappinstallstatus"></a><span data-ttu-id="11078-103">Erstellen von userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="11078-103">Create userAppInstallStatus</span></span>

> <span data-ttu-id="11078-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="11078-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11078-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="11078-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11078-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="11078-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11078-107">Erstellen eines neuen [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="11078-107">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="11078-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="11078-108">Prerequisites</span></span>
<span data-ttu-id="11078-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11078-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11078-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="11078-111">Permission type</span></span>|<span data-ttu-id="11078-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="11078-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11078-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="11078-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11078-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11078-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="11078-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="11078-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11078-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11078-116">Not supported.</span></span>|
|<span data-ttu-id="11078-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="11078-117">Application</span></span>|<span data-ttu-id="11078-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11078-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11078-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="11078-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="11078-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="11078-120">Request headers</span></span>
|<span data-ttu-id="11078-121">Header</span><span class="sxs-lookup"><span data-stu-id="11078-121">Header</span></span>|<span data-ttu-id="11078-122">Wert</span><span class="sxs-lookup"><span data-stu-id="11078-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11078-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="11078-123">Authorization</span></span>|<span data-ttu-id="11078-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="11078-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11078-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="11078-125">Accept</span></span>|<span data-ttu-id="11078-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11078-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11078-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="11078-127">Request body</span></span>
<span data-ttu-id="11078-128">Geben Sie im Textkörper Anforderung für das Objekt UserAppInstallStatus eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="11078-128">In the request body, supply a JSON representation for the userAppInstallStatus object.</span></span>

<span data-ttu-id="11078-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die UserAppInstallStatus erstellen.</span><span class="sxs-lookup"><span data-stu-id="11078-129">The following table shows the properties that are required when you create the userAppInstallStatus.</span></span>

|<span data-ttu-id="11078-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="11078-130">Property</span></span>|<span data-ttu-id="11078-131">Typ</span><span class="sxs-lookup"><span data-stu-id="11078-131">Type</span></span>|<span data-ttu-id="11078-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11078-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11078-133">id</span><span class="sxs-lookup"><span data-stu-id="11078-133">id</span></span>|<span data-ttu-id="11078-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="11078-134">String</span></span>|<span data-ttu-id="11078-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="11078-135">Key of the entity.</span></span>|
|<span data-ttu-id="11078-136">userName</span><span class="sxs-lookup"><span data-stu-id="11078-136">userName</span></span>|<span data-ttu-id="11078-137">String</span><span class="sxs-lookup"><span data-stu-id="11078-137">String</span></span>|<span data-ttu-id="11078-138">Name des Benutzers</span><span class="sxs-lookup"><span data-stu-id="11078-138">User name.</span></span>|
|<span data-ttu-id="11078-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="11078-139">userPrincipalName</span></span>|<span data-ttu-id="11078-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="11078-140">String</span></span>|<span data-ttu-id="11078-141">Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="11078-141">User Principal Name.</span></span>|
|<span data-ttu-id="11078-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="11078-142">installedDeviceCount</span></span>|<span data-ttu-id="11078-143">Int32</span><span class="sxs-lookup"><span data-stu-id="11078-143">Int32</span></span>|<span data-ttu-id="11078-144">Anzahl der installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="11078-144">Installed Device Count.</span></span>|
|<span data-ttu-id="11078-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="11078-145">failedDeviceCount</span></span>|<span data-ttu-id="11078-146">Int32</span><span class="sxs-lookup"><span data-stu-id="11078-146">Int32</span></span>|<span data-ttu-id="11078-147">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="11078-147">Failed Device Count.</span></span>|
|<span data-ttu-id="11078-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="11078-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="11078-149">Int32</span><span class="sxs-lookup"><span data-stu-id="11078-149">Int32</span></span>|<span data-ttu-id="11078-150">Anzahl der nicht installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="11078-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="11078-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="11078-151">Response</span></span>
<span data-ttu-id="11078-152">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="11078-152">If successful, this method returns a `201 Created` response code and a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11078-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="11078-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="11078-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11078-154">Request</span></span>
<span data-ttu-id="11078-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11078-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="11078-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="11078-156">Response</span></span>
<span data-ttu-id="11078-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11078-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





