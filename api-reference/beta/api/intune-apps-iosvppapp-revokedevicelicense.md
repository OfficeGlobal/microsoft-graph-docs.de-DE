---
title: RevokeDeviceLicense Aktion
description: REVOKE zugewiesen iOS VPP Gerätenlizenz für app zu reparieren.
author: tfitzmac
ms.openlocfilehash: 17ae2ed812d5c5b5a35926934d748fb730aafacf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353130"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="ab441-103">RevokeDeviceLicense Aktion</span><span class="sxs-lookup"><span data-stu-id="ab441-103">revokeDeviceLicense action</span></span>

> <span data-ttu-id="ab441-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ab441-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab441-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ab441-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab441-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ab441-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab441-107">REVOKE zugewiesen iOS VPP Gerätenlizenz für app zu reparieren.</span><span class="sxs-lookup"><span data-stu-id="ab441-107">Revoke assigned iOS VPP device license for given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab441-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ab441-108">Prerequisites</span></span>
<span data-ttu-id="ab441-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab441-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab441-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ab441-111">Permission type</span></span>|<span data-ttu-id="ab441-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ab441-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab441-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ab441-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab441-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab441-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ab441-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ab441-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab441-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab441-116">Not supported.</span></span>|
|<span data-ttu-id="ab441-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ab441-117">Application</span></span>|<span data-ttu-id="ab441-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab441-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab441-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab441-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="ab441-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ab441-120">Request headers</span></span>
|<span data-ttu-id="ab441-121">Header</span><span class="sxs-lookup"><span data-stu-id="ab441-121">Header</span></span>|<span data-ttu-id="ab441-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ab441-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab441-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ab441-123">Authorization</span></span>|<span data-ttu-id="ab441-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ab441-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab441-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab441-125">Accept</span></span>|<span data-ttu-id="ab441-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab441-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab441-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ab441-127">Request body</span></span>
<span data-ttu-id="ab441-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="ab441-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ab441-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="ab441-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ab441-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ab441-130">Property</span></span>|<span data-ttu-id="ab441-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ab441-131">Type</span></span>|<span data-ttu-id="ab441-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab441-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab441-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="ab441-133">managedDeviceId</span></span>|<span data-ttu-id="ab441-134">String</span><span class="sxs-lookup"><span data-stu-id="ab441-134">String</span></span>|<span data-ttu-id="ab441-135">Geräte-ID für die zugewiesenen app-Lizenz ist gesperrt werden</span><span class="sxs-lookup"><span data-stu-id="ab441-135">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="ab441-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="ab441-136">notifyManagedDevices</span></span>|<span data-ttu-id="ab441-137">Boolesch</span><span class="sxs-lookup"><span data-stu-id="ab441-137">Boolean</span></span>|<span data-ttu-id="ab441-138">Boolescher Wert, der angibt, ob Revoke-Benachrichtigung an Gerät gesendet werden sollen</span><span class="sxs-lookup"><span data-stu-id="ab441-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="ab441-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab441-139">Response</span></span>
<span data-ttu-id="ab441-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="ab441-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ab441-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ab441-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab441-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab441-142">Request</span></span>
<span data-ttu-id="ab441-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ab441-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="ab441-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab441-144">Response</span></span>
<span data-ttu-id="ab441-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ab441-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





