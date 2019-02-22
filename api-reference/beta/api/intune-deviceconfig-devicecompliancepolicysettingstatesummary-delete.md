---
title: deviceCompliancePolicySettingStateSummary löschen
description: Löscht ein deviceCompliancePolicySettingStateSummary-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 79c67d4053a2800fa953b40ed617154632c0ecff
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171232"
---
# <a name="delete-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="260cd-103">deviceCompliancePolicySettingStateSummary löschen</span><span class="sxs-lookup"><span data-stu-id="260cd-103">Delete deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="260cd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="260cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="260cd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="260cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="260cd-106">Löscht ein [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="260cd-106">Deletes a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="260cd-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="260cd-107">Prerequisites</span></span>
<span data-ttu-id="260cd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="260cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="260cd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="260cd-110">Permission type</span></span>|<span data-ttu-id="260cd-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="260cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="260cd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="260cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="260cd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="260cd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="260cd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="260cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="260cd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="260cd-115">Not supported.</span></span>|
|<span data-ttu-id="260cd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="260cd-116">Application</span></span>|<span data-ttu-id="260cd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="260cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="260cd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="260cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="260cd-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="260cd-119">Request headers</span></span>
|<span data-ttu-id="260cd-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="260cd-120">Header</span></span>|<span data-ttu-id="260cd-121">Wert</span><span class="sxs-lookup"><span data-stu-id="260cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="260cd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="260cd-122">Authorization</span></span>|<span data-ttu-id="260cd-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="260cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="260cd-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="260cd-124">Accept</span></span>|<span data-ttu-id="260cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="260cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="260cd-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="260cd-126">Request body</span></span>
<span data-ttu-id="260cd-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="260cd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="260cd-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="260cd-128">Response</span></span>
<span data-ttu-id="260cd-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="260cd-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="260cd-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="260cd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="260cd-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="260cd-131">Request</span></span>
<span data-ttu-id="260cd-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="260cd-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="260cd-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="260cd-133">Response</span></span>
<span data-ttu-id="260cd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="260cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




