---
title: windows10CompliancePolicy löschen
description: Löscht Objekte des Typs windows10CompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 674ec98367d7e13d90d3937ab115c1b9ad219f84
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397561"
---
# <a name="delete-windows10compliancepolicy"></a><span data-ttu-id="44857-103">windows10CompliancePolicy löschen</span><span class="sxs-lookup"><span data-stu-id="44857-103">Delete windows10CompliancePolicy</span></span>

> <span data-ttu-id="44857-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="44857-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="44857-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="44857-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44857-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="44857-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44857-107">Löscht Objekte des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="44857-107">Deletes a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44857-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="44857-108">Prerequisites</span></span>
<span data-ttu-id="44857-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="44857-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="44857-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="44857-111">Permission type</span></span>|<span data-ttu-id="44857-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="44857-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44857-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="44857-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44857-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44857-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44857-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="44857-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44857-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44857-116">Not supported.</span></span>|
|<span data-ttu-id="44857-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="44857-117">Application</span></span>|<span data-ttu-id="44857-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44857-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44857-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="44857-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="44857-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="44857-120">Request headers</span></span>
|<span data-ttu-id="44857-121">Header</span><span class="sxs-lookup"><span data-stu-id="44857-121">Header</span></span>|<span data-ttu-id="44857-122">Wert</span><span class="sxs-lookup"><span data-stu-id="44857-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44857-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="44857-123">Authorization</span></span>|<span data-ttu-id="44857-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="44857-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44857-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="44857-125">Accept</span></span>|<span data-ttu-id="44857-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44857-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44857-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="44857-127">Request body</span></span>
<span data-ttu-id="44857-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="44857-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44857-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="44857-129">Response</span></span>
<span data-ttu-id="44857-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44857-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="44857-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="44857-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="44857-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44857-132">Request</span></span>
<span data-ttu-id="44857-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44857-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="44857-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="44857-134">Response</span></span>
<span data-ttu-id="44857-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44857-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




