---
title: RevokeUserLicense Aktion
description: REVOKE zugewiesen iOS VPP-Benutzerlizenz für die app zu reparieren.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 241306b812615bb804a3139082a439df9eeae059
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837303"
---
# <a name="revokeuserlicense-action"></a><span data-ttu-id="127ad-103">RevokeUserLicense Aktion</span><span class="sxs-lookup"><span data-stu-id="127ad-103">revokeUserLicense action</span></span>

> <span data-ttu-id="127ad-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="127ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="127ad-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="127ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="127ad-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="127ad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="127ad-107">REVOKE zugewiesen iOS VPP-Benutzerlizenz für die app zu reparieren.</span><span class="sxs-lookup"><span data-stu-id="127ad-107">Revoke assigned iOS VPP user license for given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="127ad-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="127ad-108">Prerequisites</span></span>
<span data-ttu-id="127ad-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="127ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="127ad-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="127ad-111">Permission type</span></span>|<span data-ttu-id="127ad-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="127ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="127ad-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="127ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="127ad-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="127ad-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="127ad-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="127ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="127ad-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="127ad-116">Not supported.</span></span>|
|<span data-ttu-id="127ad-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="127ad-117">Application</span></span>|<span data-ttu-id="127ad-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="127ad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="127ad-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="127ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeUserLicense
```

## <a name="request-headers"></a><span data-ttu-id="127ad-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="127ad-120">Request headers</span></span>
|<span data-ttu-id="127ad-121">Header</span><span class="sxs-lookup"><span data-stu-id="127ad-121">Header</span></span>|<span data-ttu-id="127ad-122">Wert</span><span class="sxs-lookup"><span data-stu-id="127ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="127ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="127ad-123">Authorization</span></span>|<span data-ttu-id="127ad-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="127ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="127ad-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="127ad-125">Accept</span></span>|<span data-ttu-id="127ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="127ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="127ad-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="127ad-127">Request body</span></span>
<span data-ttu-id="127ad-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="127ad-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="127ad-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="127ad-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="127ad-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="127ad-130">Property</span></span>|<span data-ttu-id="127ad-131">Typ</span><span class="sxs-lookup"><span data-stu-id="127ad-131">Type</span></span>|<span data-ttu-id="127ad-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="127ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="127ad-133">userId</span><span class="sxs-lookup"><span data-stu-id="127ad-133">userId</span></span>|<span data-ttu-id="127ad-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="127ad-134">String</span></span>|<span data-ttu-id="127ad-135">Benutzer-ID für die zugewiesenen app-Lizenz ist gesperrt werden</span><span class="sxs-lookup"><span data-stu-id="127ad-135">UserId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="127ad-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="127ad-136">notifyManagedDevices</span></span>|<span data-ttu-id="127ad-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="127ad-137">Boolean</span></span>|<span data-ttu-id="127ad-138">Boolescher Wert, der angibt, ob Revoke-Benachrichtigung an Gerät gesendet werden sollen</span><span class="sxs-lookup"><span data-stu-id="127ad-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="127ad-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="127ad-139">Response</span></span>
<span data-ttu-id="127ad-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="127ad-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="127ad-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="127ad-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="127ad-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="127ad-142">Request</span></span>
<span data-ttu-id="127ad-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="127ad-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense

Content-type: application/json
Content-length: 66

{
  "userId": "User Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="127ad-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="127ad-144">Response</span></span>
<span data-ttu-id="127ad-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="127ad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





