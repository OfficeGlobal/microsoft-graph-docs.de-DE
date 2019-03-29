---
title: iosCompliancePolicy löschen
description: Löscht ein iosCompliancePolicy-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 638d4433f60faebf20d6026eda60ec7c624dd196
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974433"
---
# <a name="delete-ioscompliancepolicy"></a><span data-ttu-id="a5388-103">iosCompliancePolicy löschen</span><span class="sxs-lookup"><span data-stu-id="a5388-103">Delete iosCompliancePolicy</span></span>

> <span data-ttu-id="a5388-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a5388-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5388-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a5388-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5388-106">Löscht ein [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="a5388-106">Deletes a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5388-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a5388-107">Prerequisites</span></span>
<span data-ttu-id="a5388-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5388-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5388-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a5388-110">Permission type</span></span>|<span data-ttu-id="a5388-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a5388-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5388-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a5388-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5388-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5388-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5388-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a5388-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5388-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5388-115">Not supported.</span></span>|
|<span data-ttu-id="a5388-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a5388-116">Application</span></span>|<span data-ttu-id="a5388-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5388-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5388-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5388-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="a5388-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a5388-119">Request headers</span></span>
|<span data-ttu-id="a5388-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a5388-120">Header</span></span>|<span data-ttu-id="a5388-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a5388-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5388-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5388-122">Authorization</span></span>|<span data-ttu-id="a5388-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a5388-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5388-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a5388-124">Accept</span></span>|<span data-ttu-id="a5388-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5388-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5388-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a5388-126">Request body</span></span>
<span data-ttu-id="a5388-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a5388-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5388-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5388-128">Response</span></span>
<span data-ttu-id="a5388-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a5388-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a5388-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a5388-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5388-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5388-131">Request</span></span>
<span data-ttu-id="a5388-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a5388-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="a5388-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5388-133">Response</span></span>
<span data-ttu-id="a5388-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a5388-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




