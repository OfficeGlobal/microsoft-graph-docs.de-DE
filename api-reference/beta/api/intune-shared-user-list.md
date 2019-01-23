---
title: Benutzer auflisten
description: Auflisten von Eigenschaften und Beziehungen der user-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2ebdc1842eb3530a0327326b2c06fa87eb92563a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401859"
---
# <a name="list-users"></a><span data-ttu-id="0cb05-103">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="0cb05-103">List users</span></span>

> <span data-ttu-id="0cb05-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0cb05-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0cb05-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0cb05-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0cb05-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0cb05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cb05-107">Auflisten von Eigenschaften und Beziehungen der [user](../resources/intune-shared-user.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="0cb05-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cb05-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0cb05-108">Prerequisites</span></span>

<span data-ttu-id="0cb05-109">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="0cb05-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0cb05-110">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cb05-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="0cb05-111">Die jeweilige Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="0cb05-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="0cb05-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0cb05-112">Permission type</span></span>|<span data-ttu-id="0cb05-113">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0cb05-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cb05-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0cb05-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0cb05-115">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="0cb05-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="0cb05-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cb05-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="0cb05-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="0cb05-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="0cb05-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cb05-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="0cb05-119">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="0cb05-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="0cb05-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cb05-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="0cb05-121">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="0cb05-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="0cb05-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cb05-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="0cb05-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0cb05-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cb05-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0cb05-124">Not supported.</span></span>|
|<span data-ttu-id="0cb05-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0cb05-125">Application</span></span>|<span data-ttu-id="0cb05-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0cb05-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cb05-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0cb05-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="0cb05-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0cb05-128">Request headers</span></span>

|<span data-ttu-id="0cb05-129">Header</span><span class="sxs-lookup"><span data-stu-id="0cb05-129">Header</span></span>|<span data-ttu-id="0cb05-130">Wert</span><span class="sxs-lookup"><span data-stu-id="0cb05-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cb05-131">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0cb05-131">Authorization</span></span>|<span data-ttu-id="0cb05-132">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0cb05-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cb05-133">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0cb05-133">Accept</span></span>|<span data-ttu-id="0cb05-134">application/json</span><span class="sxs-lookup"><span data-stu-id="0cb05-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cb05-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0cb05-135">Request body</span></span>

<span data-ttu-id="0cb05-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0cb05-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cb05-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="0cb05-137">Response</span></span>

<span data-ttu-id="0cb05-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/intune-shared-user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0cb05-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cb05-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0cb05-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cb05-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0cb05-140">Request</span></span>

<span data-ttu-id="0cb05-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0cb05-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="0cb05-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="0cb05-142">Response</span></span>

<span data-ttu-id="0cb05-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0cb05-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



