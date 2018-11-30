---
title: deviceCompliancePolicySettingStateSummary löschen
description: Löscht ein deviceCompliancePolicySettingStateSummary-Objekt.
ms.openlocfilehash: 72977d504c4b5db51d88266872132db07f2ead1f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017565"
---
# <a name="delete-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="2e8a3-103">deviceCompliancePolicySettingStateSummary löschen</span><span class="sxs-lookup"><span data-stu-id="2e8a3-103">Delete deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="2e8a3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2e8a3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e8a3-105">Löscht ein [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="2e8a3-105">Deletes a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e8a3-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2e8a3-106">Prerequisites</span></span>
<span data-ttu-id="2e8a3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e8a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e8a3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e8a3-109">Permission type</span></span>|<span data-ttu-id="2e8a3-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e8a3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e8a3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e8a3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2e8a3-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e8a3-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2e8a3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e8a3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e8a3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e8a3-114">Not supported.</span></span>|
|<span data-ttu-id="2e8a3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e8a3-115">Application</span></span>|<span data-ttu-id="2e8a3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e8a3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e8a3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e8a3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="2e8a3-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e8a3-118">Request headers</span></span>
|<span data-ttu-id="2e8a3-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2e8a3-119">Header</span></span>|<span data-ttu-id="2e8a3-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2e8a3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e8a3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e8a3-121">Authorization</span></span>|<span data-ttu-id="2e8a3-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2e8a3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e8a3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2e8a3-123">Accept</span></span>|<span data-ttu-id="2e8a3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2e8a3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e8a3-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2e8a3-125">Request body</span></span>
<span data-ttu-id="2e8a3-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2e8a3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e8a3-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e8a3-127">Response</span></span>
<span data-ttu-id="2e8a3-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e8a3-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2e8a3-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e8a3-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2e8a3-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e8a3-130">Request</span></span>
<span data-ttu-id="2e8a3-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e8a3-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="2e8a3-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e8a3-132">Response</span></span>
<span data-ttu-id="2e8a3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e8a3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```


