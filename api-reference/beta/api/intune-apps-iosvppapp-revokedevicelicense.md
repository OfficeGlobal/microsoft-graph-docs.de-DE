---
title: RevokeDeviceLicense Aktion
description: REVOKE zugewiesen iOS VPP Gerätenlizenz für app zu reparieren.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 83d15f542799fb604a3d82d5ac6989087ff75bcf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979096"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="9f099-103">RevokeDeviceLicense Aktion</span><span class="sxs-lookup"><span data-stu-id="9f099-103">revokeDeviceLicense action</span></span>

> <span data-ttu-id="9f099-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9f099-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f099-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f099-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f099-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9f099-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f099-107">REVOKE zugewiesen iOS VPP Gerätenlizenz für app zu reparieren.</span><span class="sxs-lookup"><span data-stu-id="9f099-107">Revoke assigned iOS VPP device license for given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f099-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9f099-108">Prerequisites</span></span>
<span data-ttu-id="9f099-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f099-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f099-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f099-111">Permission type</span></span>|<span data-ttu-id="9f099-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f099-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f099-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f099-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f099-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f099-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9f099-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f099-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f099-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f099-116">Not supported.</span></span>|
|<span data-ttu-id="9f099-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f099-117">Application</span></span>|<span data-ttu-id="9f099-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f099-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f099-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f099-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="9f099-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f099-120">Request headers</span></span>
|<span data-ttu-id="9f099-121">Header</span><span class="sxs-lookup"><span data-stu-id="9f099-121">Header</span></span>|<span data-ttu-id="9f099-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9f099-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f099-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f099-123">Authorization</span></span>|<span data-ttu-id="9f099-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9f099-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f099-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9f099-125">Accept</span></span>|<span data-ttu-id="9f099-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f099-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f099-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f099-127">Request body</span></span>
<span data-ttu-id="9f099-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="9f099-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9f099-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="9f099-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9f099-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9f099-130">Property</span></span>|<span data-ttu-id="9f099-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9f099-131">Type</span></span>|<span data-ttu-id="9f099-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f099-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f099-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="9f099-133">managedDeviceId</span></span>|<span data-ttu-id="9f099-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9f099-134">String</span></span>|<span data-ttu-id="9f099-135">Geräte-ID für die zugewiesenen app-Lizenz ist gesperrt werden</span><span class="sxs-lookup"><span data-stu-id="9f099-135">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="9f099-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="9f099-136">notifyManagedDevices</span></span>|<span data-ttu-id="9f099-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9f099-137">Boolean</span></span>|<span data-ttu-id="9f099-138">Boolescher Wert, der angibt, ob Revoke-Benachrichtigung an Gerät gesendet werden sollen</span><span class="sxs-lookup"><span data-stu-id="9f099-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="9f099-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f099-139">Response</span></span>
<span data-ttu-id="9f099-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="9f099-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9f099-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f099-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f099-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f099-142">Request</span></span>
<span data-ttu-id="9f099-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f099-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="9f099-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f099-144">Response</span></span>
<span data-ttu-id="9f099-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f099-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





