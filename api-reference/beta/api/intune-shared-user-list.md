---
title: Benutzer auflisten
description: Auflisten von Eigenschaften und Beziehungen der user-Objekte.
author: tfitzmac
ms.openlocfilehash: ab3849bad141463bc674dce7c692d33c6e652952
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357666"
---
# <a name="list-users"></a><span data-ttu-id="b6853-103">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="b6853-103">List users</span></span>

> <span data-ttu-id="b6853-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b6853-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6853-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b6853-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6853-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b6853-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6853-107">Auflisten von Eigenschaften und Beziehungen der [user](../resources/intune-shared-user.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="b6853-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6853-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b6853-108">Prerequisites</span></span>

<span data-ttu-id="b6853-109">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="b6853-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b6853-110">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6853-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="b6853-111">Die jeweilige Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="b6853-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="b6853-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b6853-112">Permission type</span></span>|<span data-ttu-id="b6853-113">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b6853-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6853-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b6853-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b6853-115">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="b6853-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b6853-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6853-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b6853-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="b6853-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="b6853-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6853-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="b6853-119">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="b6853-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b6853-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6853-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b6853-121">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="b6853-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b6853-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6853-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="b6853-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b6853-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6853-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6853-124">Not supported.</span></span>|
|<span data-ttu-id="b6853-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b6853-125">Application</span></span>|<span data-ttu-id="b6853-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6853-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6853-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6853-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="b6853-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b6853-128">Request headers</span></span>

|<span data-ttu-id="b6853-129">Header</span><span class="sxs-lookup"><span data-stu-id="b6853-129">Header</span></span>|<span data-ttu-id="b6853-130">Wert</span><span class="sxs-lookup"><span data-stu-id="b6853-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6853-131">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b6853-131">Authorization</span></span>|<span data-ttu-id="b6853-132">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b6853-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6853-133">Accept</span><span class="sxs-lookup"><span data-stu-id="b6853-133">Accept</span></span>|<span data-ttu-id="b6853-134">application/json</span><span class="sxs-lookup"><span data-stu-id="b6853-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6853-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b6853-135">Request body</span></span>

<span data-ttu-id="b6853-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b6853-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6853-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6853-137">Response</span></span>

<span data-ttu-id="b6853-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/intune-shared-user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b6853-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6853-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b6853-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6853-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6853-140">Request</span></span>

<span data-ttu-id="b6853-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b6853-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="b6853-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6853-142">Response</span></span>

<span data-ttu-id="b6853-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b6853-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



