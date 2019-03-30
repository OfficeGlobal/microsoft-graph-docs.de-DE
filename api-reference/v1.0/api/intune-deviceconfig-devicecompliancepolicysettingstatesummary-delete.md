---
title: deviceCompliancePolicySettingStateSummary löschen
description: Löscht ein deviceCompliancePolicySettingStateSummary-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0a33ec4629b98ab5824a4c7b25e6c268d9c980d0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988343"
---
# <a name="delete-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="cad59-103">deviceCompliancePolicySettingStateSummary löschen</span><span class="sxs-lookup"><span data-stu-id="cad59-103">Delete deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="cad59-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cad59-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cad59-105">Löscht ein [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="cad59-105">Deletes a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cad59-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cad59-106">Prerequisites</span></span>
<span data-ttu-id="cad59-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cad59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cad59-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cad59-109">Permission type</span></span>|<span data-ttu-id="cad59-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cad59-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cad59-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cad59-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cad59-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cad59-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cad59-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cad59-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cad59-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cad59-114">Not supported.</span></span>|
|<span data-ttu-id="cad59-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cad59-115">Application</span></span>|<span data-ttu-id="cad59-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cad59-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cad59-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cad59-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="cad59-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cad59-118">Request headers</span></span>
|<span data-ttu-id="cad59-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cad59-119">Header</span></span>|<span data-ttu-id="cad59-120">Wert</span><span class="sxs-lookup"><span data-stu-id="cad59-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cad59-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cad59-121">Authorization</span></span>|<span data-ttu-id="cad59-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cad59-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cad59-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cad59-123">Accept</span></span>|<span data-ttu-id="cad59-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cad59-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cad59-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cad59-125">Request body</span></span>
<span data-ttu-id="cad59-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cad59-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cad59-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="cad59-127">Response</span></span>
<span data-ttu-id="cad59-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cad59-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cad59-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cad59-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="cad59-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cad59-130">Request</span></span>
<span data-ttu-id="cad59-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cad59-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="cad59-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="cad59-132">Response</span></span>
<span data-ttu-id="cad59-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cad59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



