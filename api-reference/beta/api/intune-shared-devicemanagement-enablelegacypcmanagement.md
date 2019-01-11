---
title: EnableLegacyPcManagement Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dfba24f59632126810e09dbce26970eb1c887b73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818522"
---
# <a name="enablelegacypcmanagement-action"></a><span data-ttu-id="df580-103">EnableLegacyPcManagement Aktion</span><span class="sxs-lookup"><span data-stu-id="df580-103">enableLegacyPcManagement action</span></span>

> <span data-ttu-id="df580-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="df580-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df580-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df580-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df580-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="df580-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df580-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="df580-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df580-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="df580-108">Prerequisites</span></span>
<span data-ttu-id="df580-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df580-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df580-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="df580-111">Permission type</span></span>|<span data-ttu-id="df580-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="df580-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df580-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="df580-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="df580-114">&nbsp;&nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="df580-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="df580-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df580-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df580-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="df580-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df580-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df580-117">Not supported.</span></span>|
|<span data-ttu-id="df580-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="df580-118">Application</span></span>|<span data-ttu-id="df580-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df580-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df580-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="df580-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableLegacyPcManagement
```

## <a name="request-headers"></a><span data-ttu-id="df580-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="df580-121">Request headers</span></span>
|<span data-ttu-id="df580-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="df580-122">Header</span></span>|<span data-ttu-id="df580-123">Wert</span><span class="sxs-lookup"><span data-stu-id="df580-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df580-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="df580-124">Authorization</span></span>|<span data-ttu-id="df580-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="df580-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df580-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="df580-126">Accept</span></span>|<span data-ttu-id="df580-127">application/json</span><span class="sxs-lookup"><span data-stu-id="df580-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df580-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="df580-128">Request body</span></span>
<span data-ttu-id="df580-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="df580-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df580-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="df580-130">Response</span></span>
<span data-ttu-id="df580-131">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="df580-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="df580-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="df580-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="df580-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="df580-133">Request</span></span>
<span data-ttu-id="df580-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="df580-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableLegacyPcManagement
```

### <a name="response"></a><span data-ttu-id="df580-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="df580-135">Response</span></span>
<span data-ttu-id="df580-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="df580-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





