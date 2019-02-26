---
title: windows10CompliancePolicy löschen
description: Löscht Objekte des Typs windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d13ec319204b0fbb626facf38047c37980dfecbb
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257267"
---
# <a name="delete-windows10compliancepolicy"></a><span data-ttu-id="1c761-103">windows10CompliancePolicy löschen</span><span class="sxs-lookup"><span data-stu-id="1c761-103">Delete windows10CompliancePolicy</span></span>

> <span data-ttu-id="1c761-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1c761-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c761-105">Löscht Objekte des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1c761-105">Deletes a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c761-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1c761-106">Prerequisites</span></span>
<span data-ttu-id="1c761-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1c761-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1c761-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c761-109">Permission type</span></span>|<span data-ttu-id="1c761-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c761-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c761-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c761-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1c761-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c761-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c761-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c761-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c761-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c761-114">Not supported.</span></span>|
|<span data-ttu-id="1c761-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c761-115">Application</span></span>|<span data-ttu-id="1c761-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c761-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c761-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c761-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="1c761-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c761-118">Request headers</span></span>
|<span data-ttu-id="1c761-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1c761-119">Header</span></span>|<span data-ttu-id="1c761-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1c761-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c761-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c761-121">Authorization</span></span>|<span data-ttu-id="1c761-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1c761-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c761-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1c761-123">Accept</span></span>|<span data-ttu-id="1c761-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1c761-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c761-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c761-125">Request body</span></span>
<span data-ttu-id="1c761-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1c761-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c761-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c761-127">Response</span></span>
<span data-ttu-id="1c761-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c761-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1c761-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1c761-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c761-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c761-130">Request</span></span>
<span data-ttu-id="1c761-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1c761-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="1c761-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c761-132">Response</span></span>
<span data-ttu-id="1c761-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c761-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



