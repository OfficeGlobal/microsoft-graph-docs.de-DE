---
title: EmbeddedSIMActivationCodePool löschen
description: Löscht eine EmbeddedSIMActivationCodePool.
author: tfitzmac
ms.openlocfilehash: 25d55d45f035e871de867258528303db2ba1484f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330954"
---
# <a name="delete-embeddedsimactivationcodepool"></a><span data-ttu-id="3e479-103">EmbeddedSIMActivationCodePool löschen</span><span class="sxs-lookup"><span data-stu-id="3e479-103">Delete embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="3e479-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3e479-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e479-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3e479-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e479-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3e479-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e479-107">Löscht eine [EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span><span class="sxs-lookup"><span data-stu-id="3e479-107">Deletes a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e479-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3e479-108">Prerequisites</span></span>
<span data-ttu-id="3e479-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e479-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e479-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e479-111">Permission type</span></span>|<span data-ttu-id="3e479-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e479-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e479-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e479-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e479-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e479-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e479-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e479-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e479-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e479-116">Not supported.</span></span>|
|<span data-ttu-id="3e479-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e479-117">Application</span></span>|<span data-ttu-id="3e479-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e479-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e479-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e479-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a><span data-ttu-id="3e479-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e479-120">Request headers</span></span>
|<span data-ttu-id="3e479-121">Header</span><span class="sxs-lookup"><span data-stu-id="3e479-121">Header</span></span>|<span data-ttu-id="3e479-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3e479-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e479-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3e479-123">Authorization</span></span>|<span data-ttu-id="3e479-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3e479-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e479-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3e479-125">Accept</span></span>|<span data-ttu-id="3e479-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e479-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e479-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e479-127">Request body</span></span>
<span data-ttu-id="3e479-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3e479-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e479-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e479-129">Response</span></span>
<span data-ttu-id="3e479-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e479-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3e479-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e479-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e479-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e479-132">Request</span></span>
<span data-ttu-id="3e479-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e479-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

### <a name="response"></a><span data-ttu-id="3e479-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e479-134">Response</span></span>
<span data-ttu-id="3e479-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e479-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





