---
title: Benutzer auflisten
description: Auflisten von Eigenschaften und Beziehungen der user-Objekte.
ms.openlocfilehash: 06044d50bf21e52f61a66a7e54b11c69c9e5f700
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019102"
---
# <a name="list-users"></a><span data-ttu-id="5d89c-103">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="5d89c-103">List users</span></span>

> <span data-ttu-id="5d89c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5d89c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d89c-105">Auflisten von Eigenschaften und Beziehungen der [user](../resources/intune-shared-user.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="5d89c-105">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5d89c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5d89c-106">Prerequisites</span></span>
<span data-ttu-id="5d89c-107">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="5d89c-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5d89c-108">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d89c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="5d89c-109">Die jeweilige Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="5d89c-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="5d89c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d89c-110">Permission type</span></span>|<span data-ttu-id="5d89c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d89c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d89c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d89c-112">Delegated (work or school account)</span></span>| <span data-ttu-id="5d89c-113">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="5d89c-113">_varies by context_</span></span>|
| <span data-ttu-id="5d89c-114">&nbsp;&nbsp; Gerätemanagement</span><span class="sxs-lookup"><span data-stu-id="5d89c-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="5d89c-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d89c-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="5d89c-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="5d89c-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="5d89c-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d89c-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="5d89c-118">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="5d89c-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="5d89c-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d89c-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5d89c-120">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="5d89c-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="5d89c-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d89c-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="5d89c-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d89c-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d89c-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d89c-123">Not supported.</span></span>|
|<span data-ttu-id="5d89c-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d89c-124">Application</span></span>|<span data-ttu-id="5d89c-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d89c-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d89c-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d89c-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="5d89c-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d89c-127">Request headers</span></span>
|<span data-ttu-id="5d89c-128">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5d89c-128">Header</span></span>|<span data-ttu-id="5d89c-129">Wert</span><span class="sxs-lookup"><span data-stu-id="5d89c-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d89c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d89c-130">Authorization</span></span>|<span data-ttu-id="5d89c-131">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5d89c-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d89c-132">Accept</span><span class="sxs-lookup"><span data-stu-id="5d89c-132">Accept</span></span>|<span data-ttu-id="5d89c-133">application/json</span><span class="sxs-lookup"><span data-stu-id="5d89c-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d89c-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5d89c-134">Request body</span></span>
<span data-ttu-id="5d89c-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5d89c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d89c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d89c-136">Response</span></span>
<span data-ttu-id="5d89c-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/intune-shared-user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d89c-137">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d89c-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d89c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d89c-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d89c-139">Request</span></span>
<span data-ttu-id="5d89c-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d89c-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="5d89c-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d89c-141">Response</span></span>
<span data-ttu-id="5d89c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d89c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
    }
  ]
}
```


