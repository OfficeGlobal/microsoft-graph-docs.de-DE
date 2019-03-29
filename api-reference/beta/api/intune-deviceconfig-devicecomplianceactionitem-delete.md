---
title: deviceComplianceActionItem löschen
description: Löscht ein Objekt des Typs deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a5bb4c20752f19b6e5b92126bf08bbc709a1665
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981279"
---
# <a name="delete-devicecomplianceactionitem"></a><span data-ttu-id="f8676-103">deviceComplianceActionItem löschen</span><span class="sxs-lookup"><span data-stu-id="f8676-103">Delete deviceComplianceActionItem</span></span>

> <span data-ttu-id="f8676-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8676-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8676-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f8676-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8676-106">Löscht ein Objekt des Typs [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="f8676-106">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8676-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f8676-107">Prerequisites</span></span>
<span data-ttu-id="f8676-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8676-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8676-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8676-110">Permission type</span></span>|<span data-ttu-id="f8676-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8676-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8676-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8676-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8676-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8676-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8676-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8676-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8676-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8676-115">Not supported.</span></span>|
|<span data-ttu-id="f8676-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8676-116">Application</span></span>|<span data-ttu-id="f8676-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8676-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8676-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8676-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="f8676-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8676-119">Request headers</span></span>
|<span data-ttu-id="f8676-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f8676-120">Header</span></span>|<span data-ttu-id="f8676-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f8676-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8676-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8676-122">Authorization</span></span>|<span data-ttu-id="f8676-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f8676-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8676-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f8676-124">Accept</span></span>|<span data-ttu-id="f8676-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8676-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8676-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f8676-126">Request body</span></span>
<span data-ttu-id="f8676-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f8676-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8676-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8676-128">Response</span></span>
<span data-ttu-id="f8676-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8676-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f8676-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f8676-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8676-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8676-131">Request</span></span>
<span data-ttu-id="f8676-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8676-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="f8676-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8676-133">Response</span></span>
<span data-ttu-id="f8676-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8676-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




