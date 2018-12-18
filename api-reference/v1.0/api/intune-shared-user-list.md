---
title: Benutzer auflisten
description: Auflisten von Eigenschaften und Beziehungen der user-Objekte.
author: tfitzmac
ms.openlocfilehash: 9d68b6855a80262daf359950967517a4ec8faa8c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357141"
---
# <a name="list-users"></a><span data-ttu-id="f8dc4-103">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="f8dc4-103">List users</span></span>

> <span data-ttu-id="f8dc4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f8dc4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8dc4-105">Auflisten von Eigenschaften und Beziehungen der [user](../resources/intune-shared-user.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="f8dc4-105">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8dc4-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f8dc4-106">Prerequisites</span></span>
<span data-ttu-id="f8dc4-107">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="f8dc4-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f8dc4-108">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8dc4-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="f8dc4-109">Die jeweilige Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="f8dc4-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="f8dc4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8dc4-110">Permission type</span></span>|<span data-ttu-id="f8dc4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8dc4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8dc4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8dc4-112">Delegated (work or school account)</span></span>| <span data-ttu-id="f8dc4-113">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="f8dc4-113">_varies by context_</span></span>|
| <span data-ttu-id="f8dc4-114">&nbsp;&nbsp; Gerätemanagement</span><span class="sxs-lookup"><span data-stu-id="f8dc4-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="f8dc4-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8dc4-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="f8dc4-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="f8dc4-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="f8dc4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8dc4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="f8dc4-118">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="f8dc4-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="f8dc4-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8dc4-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="f8dc4-120">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="f8dc4-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="f8dc4-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8dc4-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="f8dc4-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8dc4-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8dc4-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8dc4-123">Not supported.</span></span>|
|<span data-ttu-id="f8dc4-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8dc4-124">Application</span></span>|<span data-ttu-id="f8dc4-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8dc4-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8dc4-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8dc4-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="f8dc4-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8dc4-127">Request headers</span></span>
|<span data-ttu-id="f8dc4-128">Header</span><span class="sxs-lookup"><span data-stu-id="f8dc4-128">Header</span></span>|<span data-ttu-id="f8dc4-129">Wert</span><span class="sxs-lookup"><span data-stu-id="f8dc4-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8dc4-130">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f8dc4-130">Authorization</span></span>|<span data-ttu-id="f8dc4-131">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f8dc4-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8dc4-132">Accept</span><span class="sxs-lookup"><span data-stu-id="f8dc4-132">Accept</span></span>|<span data-ttu-id="f8dc4-133">application/json</span><span class="sxs-lookup"><span data-stu-id="f8dc4-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8dc4-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f8dc4-134">Request body</span></span>
<span data-ttu-id="f8dc4-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f8dc4-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8dc4-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8dc4-136">Response</span></span>
<span data-ttu-id="f8dc4-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/intune-shared-user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8dc4-137">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8dc4-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f8dc4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8dc4-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8dc4-139">Request</span></span>
<span data-ttu-id="f8dc4-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8dc4-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="f8dc4-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8dc4-141">Response</span></span>
<span data-ttu-id="f8dc4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8dc4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



