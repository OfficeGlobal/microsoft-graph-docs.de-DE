---
title: ExtendQualityUpdatesPause Aktion
description: Erweitern Sie für ein Windows-Update für Business Ring Qualität Updates anhalten.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d189c3adabc87bca1d03e04cbea68531c7396be5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841426"
---
# <a name="extendqualityupdatespause-action"></a><span data-ttu-id="0739d-103">ExtendQualityUpdatesPause Aktion</span><span class="sxs-lookup"><span data-stu-id="0739d-103">extendQualityUpdatesPause action</span></span>

> <span data-ttu-id="0739d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0739d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0739d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0739d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0739d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0739d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0739d-107">Erweitern Sie für ein Windows-Update für Business Ring Qualität Updates anhalten.</span><span class="sxs-lookup"><span data-stu-id="0739d-107">Extend Quality Updates Pause for a Windows Update for Business ring.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0739d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0739d-108">Prerequisites</span></span>
<span data-ttu-id="0739d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0739d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0739d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0739d-111">Permission type</span></span>|<span data-ttu-id="0739d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0739d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0739d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0739d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0739d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0739d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0739d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0739d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0739d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0739d-116">Not supported.</span></span>|
|<span data-ttu-id="0739d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0739d-117">Application</span></span>|<span data-ttu-id="0739d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0739d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0739d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0739d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendQualityUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/extendQualityUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/extendQualityUpdatesPause
```

## <a name="request-headers"></a><span data-ttu-id="0739d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0739d-120">Request headers</span></span>
|<span data-ttu-id="0739d-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0739d-121">Header</span></span>|<span data-ttu-id="0739d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0739d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0739d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0739d-123">Authorization</span></span>|<span data-ttu-id="0739d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0739d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0739d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0739d-125">Accept</span></span>|<span data-ttu-id="0739d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0739d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0739d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0739d-127">Request body</span></span>
<span data-ttu-id="0739d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0739d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0739d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0739d-129">Response</span></span>
<span data-ttu-id="0739d-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="0739d-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0739d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0739d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0739d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0739d-132">Request</span></span>
<span data-ttu-id="0739d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0739d-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendQualityUpdatesPause
```

### <a name="response"></a><span data-ttu-id="0739d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0739d-134">Response</span></span>
<span data-ttu-id="0739d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0739d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





