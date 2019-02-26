---
title: Benutzer auflisten
description: Auflisten von Eigenschaften und Beziehungen der user-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b3981047311673be8c640a35dbc862416427fa31
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252511"
---
# <a name="list-users"></a><span data-ttu-id="9976e-103">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="9976e-103">List users</span></span>

> <span data-ttu-id="9976e-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9976e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9976e-105">Auflisten von Eigenschaften und Beziehungen der [user](../resources/intune-shared-user.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="9976e-105">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9976e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9976e-106">Prerequisites</span></span>
<span data-ttu-id="9976e-107">Eine der folgenden Berechtigungen ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="9976e-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9976e-108">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9976e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="9976e-109">Die spezifische Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="9976e-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="9976e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9976e-110">Permission type</span></span>|<span data-ttu-id="9976e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9976e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9976e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9976e-112">Delegated (work or school account)</span></span>| <span data-ttu-id="9976e-113">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="9976e-113">_varies by context_</span></span>|
| <span data-ttu-id="9976e-114">&nbsp;&nbsp; Geräteverwaltung</span><span class="sxs-lookup"><span data-stu-id="9976e-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="9976e-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9976e-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="9976e-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="9976e-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="9976e-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9976e-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="9976e-118">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="9976e-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="9976e-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9976e-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="9976e-120">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="9976e-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="9976e-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9976e-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="9976e-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9976e-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9976e-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9976e-123">Not supported.</span></span>|
|<span data-ttu-id="9976e-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9976e-124">Application</span></span>|<span data-ttu-id="9976e-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9976e-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9976e-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9976e-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="9976e-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9976e-127">Request headers</span></span>
|<span data-ttu-id="9976e-128">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9976e-128">Header</span></span>|<span data-ttu-id="9976e-129">Wert</span><span class="sxs-lookup"><span data-stu-id="9976e-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9976e-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="9976e-130">Authorization</span></span>|<span data-ttu-id="9976e-131">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9976e-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9976e-132">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9976e-132">Accept</span></span>|<span data-ttu-id="9976e-133">application/json</span><span class="sxs-lookup"><span data-stu-id="9976e-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9976e-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9976e-134">Request body</span></span>
<span data-ttu-id="9976e-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9976e-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9976e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9976e-136">Response</span></span>
<span data-ttu-id="9976e-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/intune-shared-user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9976e-137">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9976e-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9976e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="9976e-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9976e-139">Request</span></span>
<span data-ttu-id="9976e-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9976e-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="9976e-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="9976e-141">Response</span></span>
<span data-ttu-id="9976e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9976e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



