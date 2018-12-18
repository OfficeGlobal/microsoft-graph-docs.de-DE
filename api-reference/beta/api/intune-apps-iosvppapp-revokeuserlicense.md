---
title: RevokeUserLicense Aktion
description: REVOKE zugewiesen iOS VPP-Benutzerlizenz für die app zu reparieren.
author: tfitzmac
ms.openlocfilehash: 94d8dff027421d5b3b1c763439dbcf4ec3d2391f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332809"
---
# <a name="revokeuserlicense-action"></a><span data-ttu-id="b7f4f-103">RevokeUserLicense Aktion</span><span class="sxs-lookup"><span data-stu-id="b7f4f-103">revokeUserLicense action</span></span>

> <span data-ttu-id="b7f4f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b7f4f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7f4f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b7f4f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7f4f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b7f4f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7f4f-107">REVOKE zugewiesen iOS VPP-Benutzerlizenz für die app zu reparieren.</span><span class="sxs-lookup"><span data-stu-id="b7f4f-107">Revoke assigned iOS VPP user license for given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b7f4f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b7f4f-108">Prerequisites</span></span>
<span data-ttu-id="b7f4f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7f4f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7f4f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b7f4f-111">Permission type</span></span>|<span data-ttu-id="b7f4f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b7f4f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7f4f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b7f4f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7f4f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7f4f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b7f4f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b7f4f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7f4f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b7f4f-116">Not supported.</span></span>|
|<span data-ttu-id="b7f4f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b7f4f-117">Application</span></span>|<span data-ttu-id="b7f4f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b7f4f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7f4f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7f4f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeUserLicense
```

## <a name="request-headers"></a><span data-ttu-id="b7f4f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b7f4f-120">Request headers</span></span>
|<span data-ttu-id="b7f4f-121">Header</span><span class="sxs-lookup"><span data-stu-id="b7f4f-121">Header</span></span>|<span data-ttu-id="b7f4f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b7f4f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7f4f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b7f4f-123">Authorization</span></span>|<span data-ttu-id="b7f4f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b7f4f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7f4f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b7f4f-125">Accept</span></span>|<span data-ttu-id="b7f4f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7f4f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7f4f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b7f4f-127">Request body</span></span>
<span data-ttu-id="b7f4f-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="b7f4f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b7f4f-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="b7f4f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b7f4f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b7f4f-130">Property</span></span>|<span data-ttu-id="b7f4f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b7f4f-131">Type</span></span>|<span data-ttu-id="b7f4f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7f4f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7f4f-133">userId</span><span class="sxs-lookup"><span data-stu-id="b7f4f-133">userId</span></span>|<span data-ttu-id="b7f4f-134">String</span><span class="sxs-lookup"><span data-stu-id="b7f4f-134">String</span></span>|<span data-ttu-id="b7f4f-135">Benutzer-ID für die zugewiesenen app-Lizenz ist gesperrt werden</span><span class="sxs-lookup"><span data-stu-id="b7f4f-135">UserId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="b7f4f-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="b7f4f-136">notifyManagedDevices</span></span>|<span data-ttu-id="b7f4f-137">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b7f4f-137">Boolean</span></span>|<span data-ttu-id="b7f4f-138">Boolescher Wert, der angibt, ob Revoke-Benachrichtigung an Gerät gesendet werden sollen</span><span class="sxs-lookup"><span data-stu-id="b7f4f-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="b7f4f-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7f4f-139">Response</span></span>
<span data-ttu-id="b7f4f-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="b7f4f-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b7f4f-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b7f4f-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b7f4f-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7f4f-142">Request</span></span>
<span data-ttu-id="b7f4f-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b7f4f-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense

Content-type: application/json
Content-length: 66

{
  "userId": "User Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="b7f4f-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7f4f-144">Response</span></span>
<span data-ttu-id="b7f4f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b7f4f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





