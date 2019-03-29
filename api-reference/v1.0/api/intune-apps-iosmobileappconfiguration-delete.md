---
title: iosMobileAppConfiguration löschen
description: Löscht eine iosMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2ee113b9d2a47f107023766bbd9f1702c179d3f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961805"
---
# <a name="delete-iosmobileappconfiguration"></a><span data-ttu-id="32939-103">iosMobileAppConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="32939-103">Delete iosMobileAppConfiguration</span></span>

> <span data-ttu-id="32939-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="32939-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32939-105">Löscht eine [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32939-105">Deletes a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32939-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="32939-106">Prerequisites</span></span>
<span data-ttu-id="32939-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32939-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32939-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="32939-109">Permission type</span></span>|<span data-ttu-id="32939-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="32939-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32939-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="32939-111">Delegated (work or school account)</span></span>|<span data-ttu-id="32939-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32939-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32939-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="32939-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32939-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32939-114">Not supported.</span></span>|
|<span data-ttu-id="32939-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="32939-115">Application</span></span>|<span data-ttu-id="32939-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32939-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32939-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="32939-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="32939-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="32939-118">Request headers</span></span>
|<span data-ttu-id="32939-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="32939-119">Header</span></span>|<span data-ttu-id="32939-120">Wert</span><span class="sxs-lookup"><span data-stu-id="32939-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32939-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="32939-121">Authorization</span></span>|<span data-ttu-id="32939-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="32939-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32939-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="32939-123">Accept</span></span>|<span data-ttu-id="32939-124">application/json</span><span class="sxs-lookup"><span data-stu-id="32939-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32939-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="32939-125">Request body</span></span>
<span data-ttu-id="32939-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="32939-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32939-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="32939-127">Response</span></span>
<span data-ttu-id="32939-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32939-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="32939-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="32939-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="32939-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="32939-130">Request</span></span>
<span data-ttu-id="32939-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="32939-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="32939-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="32939-132">Response</span></span>
<span data-ttu-id="32939-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32939-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



