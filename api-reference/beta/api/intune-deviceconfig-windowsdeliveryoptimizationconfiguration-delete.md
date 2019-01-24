---
title: WindowsDeliveryOptimizationConfiguration löschen
description: Löscht eine WindowsDeliveryOptimizationConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 12062c7eba23b78afad71dd63c4a95711ede26fd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430054"
---
# <a name="delete-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="29b10-103">WindowsDeliveryOptimizationConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="29b10-103">Delete windowsDeliveryOptimizationConfiguration</span></span>

> <span data-ttu-id="29b10-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="29b10-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="29b10-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="29b10-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29b10-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="29b10-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29b10-107">Löscht eine [WindowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29b10-107">Deletes a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29b10-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="29b10-108">Prerequisites</span></span>
<span data-ttu-id="29b10-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="29b10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="29b10-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="29b10-111">Permission type</span></span>|<span data-ttu-id="29b10-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="29b10-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29b10-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="29b10-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29b10-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29b10-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="29b10-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="29b10-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29b10-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29b10-116">Not supported.</span></span>|
|<span data-ttu-id="29b10-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="29b10-117">Application</span></span>|<span data-ttu-id="29b10-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29b10-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29b10-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="29b10-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="29b10-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="29b10-120">Request headers</span></span>
|<span data-ttu-id="29b10-121">Header</span><span class="sxs-lookup"><span data-stu-id="29b10-121">Header</span></span>|<span data-ttu-id="29b10-122">Wert</span><span class="sxs-lookup"><span data-stu-id="29b10-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29b10-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="29b10-123">Authorization</span></span>|<span data-ttu-id="29b10-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="29b10-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29b10-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="29b10-125">Accept</span></span>|<span data-ttu-id="29b10-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29b10-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29b10-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="29b10-127">Request body</span></span>
<span data-ttu-id="29b10-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="29b10-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29b10-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="29b10-129">Response</span></span>
<span data-ttu-id="29b10-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29b10-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="29b10-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29b10-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="29b10-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="29b10-132">Request</span></span>
<span data-ttu-id="29b10-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="29b10-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="29b10-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="29b10-134">Response</span></span>
<span data-ttu-id="29b10-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29b10-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



