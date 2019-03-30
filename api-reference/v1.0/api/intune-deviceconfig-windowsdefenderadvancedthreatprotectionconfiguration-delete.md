---
title: windowsDefenderAdvancedThreatProtectionConfiguration löschen
description: Löscht ein windowsDefenderAdvancedThreatProtectionConfiguration-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42b11ef625c2e31fb29d2d612f786c258d529d53
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988399"
---
# <a name="delete-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="10632-103">windowsDefenderAdvancedThreatProtectionConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="10632-103">Delete windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="10632-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="10632-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10632-105">Löscht ein [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="10632-105">Deletes a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10632-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="10632-106">Prerequisites</span></span>
<span data-ttu-id="10632-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10632-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10632-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="10632-109">Permission type</span></span>|<span data-ttu-id="10632-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="10632-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10632-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="10632-111">Delegated (work or school account)</span></span>|<span data-ttu-id="10632-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10632-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="10632-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="10632-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10632-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10632-114">Not supported.</span></span>|
|<span data-ttu-id="10632-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="10632-115">Application</span></span>|<span data-ttu-id="10632-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10632-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10632-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="10632-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="10632-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="10632-118">Request headers</span></span>
|<span data-ttu-id="10632-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="10632-119">Header</span></span>|<span data-ttu-id="10632-120">Wert</span><span class="sxs-lookup"><span data-stu-id="10632-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10632-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="10632-121">Authorization</span></span>|<span data-ttu-id="10632-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="10632-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10632-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="10632-123">Accept</span></span>|<span data-ttu-id="10632-124">application/json</span><span class="sxs-lookup"><span data-stu-id="10632-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10632-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="10632-125">Request body</span></span>
<span data-ttu-id="10632-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="10632-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10632-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="10632-127">Response</span></span>
<span data-ttu-id="10632-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10632-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="10632-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="10632-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="10632-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="10632-130">Request</span></span>
<span data-ttu-id="10632-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="10632-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="10632-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="10632-132">Response</span></span>
<span data-ttu-id="10632-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10632-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



