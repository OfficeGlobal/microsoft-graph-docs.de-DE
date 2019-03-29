---
title: revokeDeviceLicense-Aktion
description: Widerrufen der zugewiesenen iOS VPP-Gerätelizenz für eine bestimmte app.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4933c6f5e26f27711142a3a48068c585c684a3db
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982588"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="eda81-103">revokeDeviceLicense-Aktion</span><span class="sxs-lookup"><span data-stu-id="eda81-103">revokeDeviceLicense action</span></span>

> <span data-ttu-id="eda81-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eda81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eda81-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="eda81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eda81-106">Widerrufen der zugewiesenen iOS VPP-Gerätelizenz für eine bestimmte app.</span><span class="sxs-lookup"><span data-stu-id="eda81-106">Revoke assigned iOS VPP device license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eda81-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eda81-107">Prerequisites</span></span>
<span data-ttu-id="eda81-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eda81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eda81-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eda81-110">Permission type</span></span>|<span data-ttu-id="eda81-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eda81-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eda81-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eda81-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eda81-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eda81-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eda81-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eda81-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eda81-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eda81-115">Not supported.</span></span>|
|<span data-ttu-id="eda81-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eda81-116">Application</span></span>|<span data-ttu-id="eda81-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eda81-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eda81-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eda81-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="eda81-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eda81-119">Request headers</span></span>
|<span data-ttu-id="eda81-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eda81-120">Header</span></span>|<span data-ttu-id="eda81-121">Wert</span><span class="sxs-lookup"><span data-stu-id="eda81-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eda81-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eda81-122">Authorization</span></span>|<span data-ttu-id="eda81-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eda81-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eda81-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eda81-124">Accept</span></span>|<span data-ttu-id="eda81-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eda81-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eda81-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eda81-126">Request body</span></span>
<span data-ttu-id="eda81-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="eda81-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="eda81-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="eda81-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="eda81-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eda81-129">Property</span></span>|<span data-ttu-id="eda81-130">Typ</span><span class="sxs-lookup"><span data-stu-id="eda81-130">Type</span></span>|<span data-ttu-id="eda81-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eda81-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eda81-132">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="eda81-132">managedDeviceId</span></span>|<span data-ttu-id="eda81-133">String</span><span class="sxs-lookup"><span data-stu-id="eda81-133">String</span></span>|<span data-ttu-id="eda81-134">Geräte-Nr, für die die zugewiesene App-Lizenz widerrufen werden soll</span><span class="sxs-lookup"><span data-stu-id="eda81-134">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="eda81-135">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="eda81-135">notifyManagedDevices</span></span>|<span data-ttu-id="eda81-136">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eda81-136">Boolean</span></span>|<span data-ttu-id="eda81-137">Boolescher Wert, der angibt, ob REVOKE-Benachrichtigung an Gerät gesendet werden soll</span><span class="sxs-lookup"><span data-stu-id="eda81-137">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="eda81-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="eda81-138">Response</span></span>
<span data-ttu-id="eda81-139">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eda81-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eda81-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eda81-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="eda81-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eda81-141">Request</span></span>
<span data-ttu-id="eda81-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eda81-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="eda81-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="eda81-143">Response</span></span>
<span data-ttu-id="eda81-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eda81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




