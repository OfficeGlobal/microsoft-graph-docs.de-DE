---
title: managedAppOperation löschen
description: Löscht ein managedAppOperation-Objekt.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5ff02c7556657b9c20a5627a846a62cd03ef9dcb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841937"
---
# <a name="delete-managedappoperation"></a><span data-ttu-id="a2a4a-103">managedAppOperation löschen</span><span class="sxs-lookup"><span data-stu-id="a2a4a-103">Delete managedAppOperation</span></span>

> <span data-ttu-id="a2a4a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a2a4a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2a4a-105">Löscht ein [managedAppOperation](../resources/intune-mam-managedappoperation.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="a2a4a-105">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2a4a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a2a4a-106">Prerequisites</span></span>
<span data-ttu-id="a2a4a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2a4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2a4a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a2a4a-109">Permission type</span></span>|<span data-ttu-id="a2a4a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a2a4a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2a4a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a2a4a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a2a4a-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2a4a-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a2a4a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a2a4a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2a4a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2a4a-114">Not supported.</span></span>|
|<span data-ttu-id="a2a4a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a2a4a-115">Application</span></span>|<span data-ttu-id="a2a4a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2a4a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2a4a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2a4a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="a2a4a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a2a4a-118">Request headers</span></span>
|<span data-ttu-id="a2a4a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a2a4a-119">Header</span></span>|<span data-ttu-id="a2a4a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a2a4a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2a4a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2a4a-121">Authorization</span></span>|<span data-ttu-id="a2a4a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a2a4a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2a4a-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a2a4a-123">Accept</span></span>|<span data-ttu-id="a2a4a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a2a4a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2a4a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a2a4a-125">Request body</span></span>
<span data-ttu-id="a2a4a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a2a4a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2a4a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2a4a-127">Response</span></span>
<span data-ttu-id="a2a4a-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2a4a-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a2a4a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a2a4a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2a4a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2a4a-130">Request</span></span>
<span data-ttu-id="a2a4a-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a2a4a-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

### <a name="response"></a><span data-ttu-id="a2a4a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2a4a-132">Response</span></span>
<span data-ttu-id="a2a4a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2a4a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



