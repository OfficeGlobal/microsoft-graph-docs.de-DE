---
title: Benutzer abrufen
description: Lesen von Eigenschaften und Beziehungen des user-Objekts.
author: tfitzmac
ms.openlocfilehash: b58485112929f39be76f1f908f3097d8971ac564
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303304"
---
# <a name="get-user"></a><span data-ttu-id="80a0a-103">Benutzer abrufen</span><span class="sxs-lookup"><span data-stu-id="80a0a-103">Get user</span></span>

> <span data-ttu-id="80a0a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="80a0a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80a0a-105">Lesen von Eigenschaften und Beziehungen des [user](../resources/intune-shared-user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="80a0a-105">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80a0a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="80a0a-106">Prerequisites</span></span>
<span data-ttu-id="80a0a-107">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="80a0a-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="80a0a-108">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80a0a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="80a0a-109">Die jeweilige Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="80a0a-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="80a0a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80a0a-110">Permission type</span></span>|<span data-ttu-id="80a0a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80a0a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80a0a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80a0a-112">Delegated (work or school account)</span></span>| <span data-ttu-id="80a0a-113">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="80a0a-113">_varies by context_</span></span>|
| <span data-ttu-id="80a0a-114">&nbsp;&nbsp; Gerätemanagement</span><span class="sxs-lookup"><span data-stu-id="80a0a-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="80a0a-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="80a0a-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="80a0a-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="80a0a-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="80a0a-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="80a0a-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="80a0a-118">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="80a0a-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="80a0a-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="80a0a-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="80a0a-120">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="80a0a-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="80a0a-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="80a0a-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="80a0a-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80a0a-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80a0a-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80a0a-123">Not supported.</span></span>|
|<span data-ttu-id="80a0a-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80a0a-124">Application</span></span>|<span data-ttu-id="80a0a-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80a0a-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80a0a-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80a0a-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80a0a-127">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="80a0a-127">Optional query parameters</span></span>
<span data-ttu-id="80a0a-128">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="80a0a-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="80a0a-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80a0a-129">Request headers</span></span>
|<span data-ttu-id="80a0a-130">Header</span><span class="sxs-lookup"><span data-stu-id="80a0a-130">Header</span></span>|<span data-ttu-id="80a0a-131">Wert</span><span class="sxs-lookup"><span data-stu-id="80a0a-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80a0a-132">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="80a0a-132">Authorization</span></span>|<span data-ttu-id="80a0a-133">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="80a0a-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80a0a-134">Accept</span><span class="sxs-lookup"><span data-stu-id="80a0a-134">Accept</span></span>|<span data-ttu-id="80a0a-135">application/json</span><span class="sxs-lookup"><span data-stu-id="80a0a-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80a0a-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80a0a-136">Request body</span></span>
<span data-ttu-id="80a0a-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="80a0a-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80a0a-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="80a0a-138">Response</span></span>
<span data-ttu-id="80a0a-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/intune-shared-user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80a0a-139">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80a0a-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80a0a-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="80a0a-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="80a0a-141">Request</span></span>
<span data-ttu-id="80a0a-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80a0a-142">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="80a0a-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="80a0a-143">Response</span></span>
<span data-ttu-id="80a0a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80a0a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```



