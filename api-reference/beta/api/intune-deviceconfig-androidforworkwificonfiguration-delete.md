---
title: AndroidForWorkWiFiConfiguration löschen
description: Löscht eine androidForWorkWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 031e7184ddc46498236e10f63e73b521751472b8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976232"
---
# <a name="delete-androidforworkwificonfiguration"></a><span data-ttu-id="c0712-103">AndroidForWorkWiFiConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="c0712-103">Delete androidForWorkWiFiConfiguration</span></span>

> <span data-ttu-id="c0712-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0712-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0712-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c0712-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0712-106">Löscht eine [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0712-106">Deletes a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0712-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c0712-107">Prerequisites</span></span>
<span data-ttu-id="c0712-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0712-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0712-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0712-110">Permission type</span></span>|<span data-ttu-id="c0712-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0712-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0712-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0712-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0712-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0712-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0712-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0712-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0712-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0712-115">Not supported.</span></span>|
|<span data-ttu-id="c0712-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0712-116">Application</span></span>|<span data-ttu-id="c0712-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0712-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0712-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0712-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c0712-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0712-119">Request headers</span></span>
|<span data-ttu-id="c0712-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c0712-120">Header</span></span>|<span data-ttu-id="c0712-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c0712-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0712-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0712-122">Authorization</span></span>|<span data-ttu-id="c0712-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c0712-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0712-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c0712-124">Accept</span></span>|<span data-ttu-id="c0712-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0712-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0712-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0712-126">Request body</span></span>
<span data-ttu-id="c0712-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c0712-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0712-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0712-128">Response</span></span>
<span data-ttu-id="c0712-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0712-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c0712-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0712-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0712-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0712-131">Request</span></span>
<span data-ttu-id="c0712-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c0712-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c0712-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0712-133">Response</span></span>
<span data-ttu-id="c0712-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0712-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




