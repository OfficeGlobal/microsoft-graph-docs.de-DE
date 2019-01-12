---
title: androidCompliancePolicy löschen
description: Löscht Objekte des Typs androidCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e1a93810c4b4fb9398148665af6cba62a2b2255d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987804"
---
# <a name="delete-androidcompliancepolicy"></a><span data-ttu-id="bb001-103">androidCompliancePolicy löschen</span><span class="sxs-lookup"><span data-stu-id="bb001-103">Delete androidCompliancePolicy</span></span>

> <span data-ttu-id="bb001-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bb001-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb001-105">Löscht Objekte des Typs [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bb001-105">Deletes a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bb001-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bb001-106">Prerequisites</span></span>
<span data-ttu-id="bb001-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb001-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb001-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bb001-109">Permission type</span></span>|<span data-ttu-id="bb001-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bb001-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb001-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bb001-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb001-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb001-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb001-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bb001-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb001-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb001-114">Not supported.</span></span>|
|<span data-ttu-id="bb001-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bb001-115">Application</span></span>|<span data-ttu-id="bb001-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb001-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb001-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb001-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="bb001-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bb001-118">Request headers</span></span>
|<span data-ttu-id="bb001-119">Header</span><span class="sxs-lookup"><span data-stu-id="bb001-119">Header</span></span>|<span data-ttu-id="bb001-120">Wert</span><span class="sxs-lookup"><span data-stu-id="bb001-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb001-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb001-121">Authorization</span></span>|<span data-ttu-id="bb001-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bb001-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb001-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bb001-123">Accept</span></span>|<span data-ttu-id="bb001-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bb001-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb001-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bb001-125">Request body</span></span>
<span data-ttu-id="bb001-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bb001-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb001-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb001-127">Response</span></span>
<span data-ttu-id="bb001-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb001-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bb001-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bb001-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb001-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb001-130">Request</span></span>
<span data-ttu-id="bb001-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bb001-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="bb001-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb001-132">Response</span></span>
<span data-ttu-id="bb001-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb001-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



