---
title: iosMobileAppConfiguration löschen
description: Löscht eine iosMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 68adc2e68c396d7a09f273717934e67676c6a742
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865164"
---
# <a name="delete-iosmobileappconfiguration"></a><span data-ttu-id="a4a49-103">iosMobileAppConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="a4a49-103">Delete iosMobileAppConfiguration</span></span>

> <span data-ttu-id="a4a49-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a4a49-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4a49-105">Löscht eine [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4a49-105">Deletes a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a4a49-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a4a49-106">Prerequisites</span></span>
<span data-ttu-id="a4a49-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4a49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4a49-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a4a49-109">Permission type</span></span>|<span data-ttu-id="a4a49-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a4a49-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4a49-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a4a49-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4a49-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4a49-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a4a49-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a4a49-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4a49-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a4a49-114">Not supported.</span></span>|
|<span data-ttu-id="a4a49-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a4a49-115">Application</span></span>|<span data-ttu-id="a4a49-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a4a49-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4a49-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a4a49-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a4a49-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a4a49-118">Request headers</span></span>
|<span data-ttu-id="a4a49-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a4a49-119">Header</span></span>|<span data-ttu-id="a4a49-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a4a49-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4a49-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4a49-121">Authorization</span></span>|<span data-ttu-id="a4a49-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a4a49-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4a49-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a4a49-123">Accept</span></span>|<span data-ttu-id="a4a49-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a4a49-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4a49-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a4a49-125">Request body</span></span>
<span data-ttu-id="a4a49-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a4a49-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4a49-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a4a49-127">Response</span></span>
<span data-ttu-id="a4a49-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a4a49-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a4a49-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a4a49-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a4a49-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a4a49-130">Request</span></span>
<span data-ttu-id="a4a49-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a4a49-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a4a49-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a4a49-132">Response</span></span>
<span data-ttu-id="a4a49-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a4a49-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



