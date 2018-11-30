---
title: WindowsDomainJoinConfiguration löschen
description: Löscht eine WindowsDomainJoinConfiguration.
ms.openlocfilehash: 79126f49689ce9a25b6a0efe8e99e2427225403f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065347"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="56823-103">WindowsDomainJoinConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="56823-103">Delete windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="56823-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="56823-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56823-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="56823-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56823-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="56823-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56823-107">Löscht eine [WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="56823-107">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56823-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="56823-108">Prerequisites</span></span>
<span data-ttu-id="56823-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56823-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56823-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="56823-111">Permission type</span></span>|<span data-ttu-id="56823-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="56823-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56823-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="56823-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="56823-114">&nbsp;&nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="56823-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="56823-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56823-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="56823-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="56823-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56823-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56823-117">Not supported.</span></span>|
|<span data-ttu-id="56823-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="56823-118">Application</span></span>|<span data-ttu-id="56823-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56823-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56823-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="56823-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="56823-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="56823-121">Request headers</span></span>
|<span data-ttu-id="56823-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="56823-122">Header</span></span>|<span data-ttu-id="56823-123">Wert</span><span class="sxs-lookup"><span data-stu-id="56823-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56823-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="56823-124">Authorization</span></span>|<span data-ttu-id="56823-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="56823-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56823-126">Accept</span><span class="sxs-lookup"><span data-stu-id="56823-126">Accept</span></span>|<span data-ttu-id="56823-127">application/json</span><span class="sxs-lookup"><span data-stu-id="56823-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56823-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="56823-128">Request body</span></span>
<span data-ttu-id="56823-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="56823-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56823-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="56823-130">Response</span></span>
<span data-ttu-id="56823-131">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56823-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="56823-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="56823-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="56823-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="56823-133">Request</span></span>
<span data-ttu-id="56823-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="56823-134">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="56823-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="56823-135">Response</span></span>
<span data-ttu-id="56823-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56823-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



