---
title: Aktion „sync“
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: fd6814c99b188e6c0e8859d7035a533ce6d0b0e3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332578"
---
# <a name="sync-action"></a><span data-ttu-id="4dcbf-103">Aktion „sync“</span><span class="sxs-lookup"><span data-stu-id="4dcbf-103">sync action</span></span>

> <span data-ttu-id="4dcbf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4dcbf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4dcbf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4dcbf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4dcbf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4dcbf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4dcbf-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4dcbf-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4dcbf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4dcbf-108">Prerequisites</span></span>
<span data-ttu-id="4dcbf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dcbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dcbf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4dcbf-111">Permission type</span></span>|<span data-ttu-id="4dcbf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4dcbf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dcbf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4dcbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4dcbf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dcbf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4dcbf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4dcbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dcbf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4dcbf-116">Not supported.</span></span>|
|<span data-ttu-id="4dcbf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4dcbf-117">Application</span></span>|<span data-ttu-id="4dcbf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4dcbf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dcbf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4dcbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotSettings/sync
```

## <a name="request-headers"></a><span data-ttu-id="4dcbf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4dcbf-120">Request headers</span></span>
|<span data-ttu-id="4dcbf-121">Header</span><span class="sxs-lookup"><span data-stu-id="4dcbf-121">Header</span></span>|<span data-ttu-id="4dcbf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4dcbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dcbf-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4dcbf-123">Authorization</span></span>|<span data-ttu-id="4dcbf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4dcbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dcbf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4dcbf-125">Accept</span></span>|<span data-ttu-id="4dcbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4dcbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dcbf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4dcbf-127">Request body</span></span>
<span data-ttu-id="4dcbf-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4dcbf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4dcbf-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4dcbf-129">Response</span></span>
<span data-ttu-id="4dcbf-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="4dcbf-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4dcbf-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4dcbf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4dcbf-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4dcbf-132">Request</span></span>
<span data-ttu-id="4dcbf-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4dcbf-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings/sync
```

### <a name="response"></a><span data-ttu-id="4dcbf-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4dcbf-134">Response</span></span>
<span data-ttu-id="4dcbf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4dcbf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





