---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration löschen
description: Löscht ein deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekt.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a69b4a786fdced748da7bdd224185ef7d0a3057a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826936"
---
# <a name="delete-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="5f3db-103">deviceEnrollmentWindowsHelloForBusinessConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="5f3db-103">Delete deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="5f3db-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5f3db-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f3db-105">Löscht ein [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="5f3db-105">Deletes a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f3db-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5f3db-106">Prerequisites</span></span>
<span data-ttu-id="5f3db-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f3db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f3db-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5f3db-109">Permission type</span></span>|<span data-ttu-id="5f3db-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5f3db-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f3db-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5f3db-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5f3db-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f3db-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5f3db-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5f3db-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f3db-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f3db-114">Not supported.</span></span>|
|<span data-ttu-id="5f3db-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5f3db-115">Application</span></span>|<span data-ttu-id="5f3db-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f3db-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f3db-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f3db-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5f3db-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5f3db-118">Request headers</span></span>
|<span data-ttu-id="5f3db-119">Header</span><span class="sxs-lookup"><span data-stu-id="5f3db-119">Header</span></span>|<span data-ttu-id="5f3db-120">Wert</span><span class="sxs-lookup"><span data-stu-id="5f3db-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f3db-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f3db-121">Authorization</span></span>|<span data-ttu-id="5f3db-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5f3db-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f3db-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5f3db-123">Accept</span></span>|<span data-ttu-id="5f3db-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5f3db-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f3db-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5f3db-125">Request body</span></span>
<span data-ttu-id="5f3db-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5f3db-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f3db-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f3db-127">Response</span></span>
<span data-ttu-id="5f3db-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f3db-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5f3db-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5f3db-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f3db-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f3db-130">Request</span></span>
<span data-ttu-id="5f3db-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5f3db-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5f3db-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f3db-132">Response</span></span>
<span data-ttu-id="5f3db-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f3db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



