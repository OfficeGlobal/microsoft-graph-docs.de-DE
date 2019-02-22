---
title: revokeDeviceLicense-Aktion
description: Widerrufen der zugewiesenen iOS VPP-Gerätelizenz für eine bestimmte app.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0d00dfb436945583baaf276c8c5425fe3223df7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174804"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="a9b73-103">revokeDeviceLicense-Aktion</span><span class="sxs-lookup"><span data-stu-id="a9b73-103">revokeDeviceLicense action</span></span>

> <span data-ttu-id="a9b73-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a9b73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9b73-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a9b73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9b73-106">Widerrufen der zugewiesenen iOS VPP-Gerätelizenz für eine bestimmte app.</span><span class="sxs-lookup"><span data-stu-id="a9b73-106">Revoke assigned iOS VPP device license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9b73-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a9b73-107">Prerequisites</span></span>
<span data-ttu-id="a9b73-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a9b73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a9b73-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a9b73-110">Permission type</span></span>|<span data-ttu-id="a9b73-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a9b73-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9b73-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a9b73-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9b73-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9b73-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a9b73-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a9b73-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9b73-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a9b73-115">Not supported.</span></span>|
|<span data-ttu-id="a9b73-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a9b73-116">Application</span></span>|<span data-ttu-id="a9b73-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a9b73-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9b73-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9b73-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="a9b73-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a9b73-119">Request headers</span></span>
|<span data-ttu-id="a9b73-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a9b73-120">Header</span></span>|<span data-ttu-id="a9b73-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a9b73-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9b73-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9b73-122">Authorization</span></span>|<span data-ttu-id="a9b73-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a9b73-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9b73-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a9b73-124">Accept</span></span>|<span data-ttu-id="a9b73-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9b73-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9b73-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a9b73-126">Request body</span></span>
<span data-ttu-id="a9b73-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="a9b73-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a9b73-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="a9b73-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a9b73-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a9b73-129">Property</span></span>|<span data-ttu-id="a9b73-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a9b73-130">Type</span></span>|<span data-ttu-id="a9b73-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a9b73-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9b73-132">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="a9b73-132">managedDeviceId</span></span>|<span data-ttu-id="a9b73-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9b73-133">String</span></span>|<span data-ttu-id="a9b73-134">Geräte-Nr, für die die zugewiesene App-Lizenz widerrufen werden soll</span><span class="sxs-lookup"><span data-stu-id="a9b73-134">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="a9b73-135">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="a9b73-135">notifyManagedDevices</span></span>|<span data-ttu-id="a9b73-136">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a9b73-136">Boolean</span></span>|<span data-ttu-id="a9b73-137">Boolescher Wert, der angibt, ob REVOKE-Benachrichtigung an Gerät gesendet werden soll</span><span class="sxs-lookup"><span data-stu-id="a9b73-137">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="a9b73-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9b73-138">Response</span></span>
<span data-ttu-id="a9b73-139">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="a9b73-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a9b73-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a9b73-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9b73-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9b73-141">Request</span></span>
<span data-ttu-id="a9b73-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a9b73-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="a9b73-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9b73-143">Response</span></span>
<span data-ttu-id="a9b73-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a9b73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




