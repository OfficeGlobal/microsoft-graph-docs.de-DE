---
title: enableLegacyPcManagement-Aktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 917a7c675173d0b110ef12da01bb35ff4c101cf3
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571242"
---
# <a name="enablelegacypcmanagement-action"></a><span data-ttu-id="47d04-103">enableLegacyPcManagement-Aktion</span><span class="sxs-lookup"><span data-stu-id="47d04-103">enableLegacyPcManagement action</span></span>

> <span data-ttu-id="47d04-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="47d04-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="47d04-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="47d04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47d04-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="47d04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47d04-107">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="47d04-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47d04-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="47d04-108">Prerequisites</span></span>
<span data-ttu-id="47d04-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="47d04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="47d04-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="47d04-111">Permission type</span></span>|<span data-ttu-id="47d04-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="47d04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47d04-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="47d04-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="47d04-114">&nbsp; &nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="47d04-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="47d04-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d04-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47d04-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="47d04-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47d04-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47d04-117">Not supported.</span></span>|
|<span data-ttu-id="47d04-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="47d04-118">Application</span></span>|<span data-ttu-id="47d04-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47d04-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47d04-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="47d04-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableLegacyPcManagement
```

## <a name="request-headers"></a><span data-ttu-id="47d04-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="47d04-121">Request headers</span></span>
|<span data-ttu-id="47d04-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="47d04-122">Header</span></span>|<span data-ttu-id="47d04-123">Wert</span><span class="sxs-lookup"><span data-stu-id="47d04-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47d04-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="47d04-124">Authorization</span></span>|<span data-ttu-id="47d04-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="47d04-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47d04-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="47d04-126">Accept</span></span>|<span data-ttu-id="47d04-127">application/json</span><span class="sxs-lookup"><span data-stu-id="47d04-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47d04-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="47d04-128">Request body</span></span>
<span data-ttu-id="47d04-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="47d04-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47d04-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="47d04-130">Response</span></span>
<span data-ttu-id="47d04-131">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="47d04-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="47d04-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="47d04-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="47d04-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="47d04-133">Request</span></span>
<span data-ttu-id="47d04-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="47d04-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableLegacyPcManagement
```

### <a name="response"></a><span data-ttu-id="47d04-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="47d04-135">Response</span></span>
<span data-ttu-id="47d04-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="47d04-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





