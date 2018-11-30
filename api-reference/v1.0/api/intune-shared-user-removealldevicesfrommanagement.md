---
title: removeAllDevicesFromManagement-Aktion
description: Die Verwaltung aller Geräte für diesen Benutzer einstellen.
ms.openlocfilehash: 973c9ccba2829161189595f58e918e3be1790476
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017105"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="921d5-103">removeAllDevicesFromManagement-Aktion</span><span class="sxs-lookup"><span data-stu-id="921d5-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="921d5-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="921d5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="921d5-105">Die Verwaltung aller Geräte für diesen Benutzer einstellen.</span><span class="sxs-lookup"><span data-stu-id="921d5-105">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="921d5-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="921d5-106">Prerequisites</span></span>
<span data-ttu-id="921d5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="921d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="921d5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="921d5-109">Permission type</span></span>|<span data-ttu-id="921d5-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="921d5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="921d5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="921d5-111">Delegated (work or school account)</span></span>| <span data-ttu-id="921d5-112">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="921d5-112">_varies by context_</span></span> |
| <span data-ttu-id="921d5-113">&nbsp;&nbsp; Gerätemanagement</span><span class="sxs-lookup"><span data-stu-id="921d5-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="921d5-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="921d5-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="921d5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="921d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="921d5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="921d5-116">Not supported.</span></span>|
|<span data-ttu-id="921d5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="921d5-117">Application</span></span>|<span data-ttu-id="921d5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="921d5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="921d5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="921d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="921d5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="921d5-120">Request headers</span></span>
|<span data-ttu-id="921d5-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="921d5-121">Header</span></span>|<span data-ttu-id="921d5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="921d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="921d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="921d5-123">Authorization</span></span>|<span data-ttu-id="921d5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="921d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="921d5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="921d5-125">Accept</span></span>|<span data-ttu-id="921d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="921d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="921d5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="921d5-127">Request body</span></span>
<span data-ttu-id="921d5-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="921d5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="921d5-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="921d5-129">Response</span></span>
<span data-ttu-id="921d5-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="921d5-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="921d5-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="921d5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="921d5-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="921d5-132">Request</span></span>
<span data-ttu-id="921d5-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="921d5-133">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="921d5-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="921d5-134">Response</span></span>
<span data-ttu-id="921d5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="921d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



