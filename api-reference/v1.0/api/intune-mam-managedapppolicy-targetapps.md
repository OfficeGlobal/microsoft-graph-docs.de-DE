---
title: targetApps-Aktion
description: Noch nicht dokumentiert
ms.openlocfilehash: 532e928dace6f956cbe17865128e5831d845abf4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018829"
---
# <a name="targetapps-action"></a><span data-ttu-id="3d013-103">targetApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="3d013-103">targetApps action</span></span>

> <span data-ttu-id="3d013-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3d013-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d013-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3d013-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3d013-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3d013-106">Prerequisites</span></span>
<span data-ttu-id="3d013-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d013-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d013-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3d013-109">Permission type</span></span>|<span data-ttu-id="3d013-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3d013-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d013-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3d013-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3d013-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d013-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3d013-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3d013-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d013-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d013-114">Not supported.</span></span>|
|<span data-ttu-id="3d013-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3d013-115">Application</span></span>|<span data-ttu-id="3d013-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d013-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d013-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d013-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="3d013-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3d013-118">Request headers</span></span>
|<span data-ttu-id="3d013-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3d013-119">Header</span></span>|<span data-ttu-id="3d013-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3d013-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d013-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d013-121">Authorization</span></span>|<span data-ttu-id="3d013-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3d013-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d013-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3d013-123">Accept</span></span>|<span data-ttu-id="3d013-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3d013-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d013-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3d013-125">Request body</span></span>
<span data-ttu-id="3d013-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="3d013-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3d013-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="3d013-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3d013-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3d013-128">Property</span></span>|<span data-ttu-id="3d013-129">Typ</span><span class="sxs-lookup"><span data-stu-id="3d013-129">Type</span></span>|<span data-ttu-id="3d013-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d013-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d013-131">Apps</span><span class="sxs-lookup"><span data-stu-id="3d013-131">apps</span></span>|<span data-ttu-id="3d013-132">Sammlung von Objekten des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d013-132">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="3d013-133">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3d013-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3d013-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d013-134">Response</span></span>
<span data-ttu-id="3d013-135">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="3d013-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3d013-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3d013-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="3d013-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d013-137">Request</span></span>
<span data-ttu-id="3d013-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3d013-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="3d013-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d013-139">Response</span></span>
<span data-ttu-id="3d013-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3d013-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```


