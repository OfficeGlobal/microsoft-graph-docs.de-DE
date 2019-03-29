---
title: WindowsDomainJoinConfiguration löschen
description: Löscht eine windowsDomainJoinConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 74cc1c53712bd20406209fc7ceca47d5eceb5786
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963037"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="b57a7-103">WindowsDomainJoinConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="b57a7-103">Delete windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="b57a7-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="b57a7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b57a7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b57a7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b57a7-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b57a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b57a7-107">Löscht eine [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b57a7-107">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b57a7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b57a7-108">Prerequisites</span></span>
<span data-ttu-id="b57a7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b57a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b57a7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b57a7-111">Permission type</span></span>|<span data-ttu-id="b57a7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b57a7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b57a7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b57a7-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b57a7-114">&nbsp; &nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="b57a7-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b57a7-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b57a7-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="b57a7-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b57a7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b57a7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b57a7-117">Not supported.</span></span>|
|<span data-ttu-id="b57a7-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b57a7-118">Application</span></span>|<span data-ttu-id="b57a7-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b57a7-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b57a7-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b57a7-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b57a7-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b57a7-121">Request headers</span></span>
|<span data-ttu-id="b57a7-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b57a7-122">Header</span></span>|<span data-ttu-id="b57a7-123">Wert</span><span class="sxs-lookup"><span data-stu-id="b57a7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b57a7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b57a7-124">Authorization</span></span>|<span data-ttu-id="b57a7-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b57a7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b57a7-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b57a7-126">Accept</span></span>|<span data-ttu-id="b57a7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b57a7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b57a7-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b57a7-128">Request body</span></span>
<span data-ttu-id="b57a7-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b57a7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b57a7-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="b57a7-130">Response</span></span>
<span data-ttu-id="b57a7-131">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b57a7-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b57a7-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b57a7-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="b57a7-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b57a7-133">Request</span></span>
<span data-ttu-id="b57a7-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b57a7-134">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b57a7-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="b57a7-135">Response</span></span>
<span data-ttu-id="b57a7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b57a7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



