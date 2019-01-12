---
title: iosUpdateConfiguration löschen
description: Löscht ein iosUpdateConfiguration-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 58402f8b56bbc1450103f8dd3a162132fc72afc7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941744"
---
# <a name="delete-iosupdateconfiguration"></a><span data-ttu-id="e1c3d-103">iosUpdateConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="e1c3d-103">Delete iosUpdateConfiguration</span></span>

> <span data-ttu-id="e1c3d-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e1c3d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1c3d-105">Löscht ein [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="e1c3d-105">Deletes a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1c3d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e1c3d-106">Prerequisites</span></span>
<span data-ttu-id="e1c3d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1c3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1c3d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1c3d-109">Permission type</span></span>|<span data-ttu-id="e1c3d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1c3d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1c3d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1c3d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e1c3d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1c3d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1c3d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1c3d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1c3d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1c3d-114">Not supported.</span></span>|
|<span data-ttu-id="e1c3d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1c3d-115">Application</span></span>|<span data-ttu-id="e1c3d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1c3d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1c3d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1c3d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e1c3d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1c3d-118">Request headers</span></span>
|<span data-ttu-id="e1c3d-119">Header</span><span class="sxs-lookup"><span data-stu-id="e1c3d-119">Header</span></span>|<span data-ttu-id="e1c3d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e1c3d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1c3d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1c3d-121">Authorization</span></span>|<span data-ttu-id="e1c3d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e1c3d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1c3d-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e1c3d-123">Accept</span></span>|<span data-ttu-id="e1c3d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e1c3d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1c3d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1c3d-125">Request body</span></span>
<span data-ttu-id="e1c3d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e1c3d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1c3d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1c3d-127">Response</span></span>
<span data-ttu-id="e1c3d-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1c3d-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e1c3d-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1c3d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1c3d-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1c3d-130">Request</span></span>
<span data-ttu-id="e1c3d-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1c3d-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e1c3d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1c3d-132">Response</span></span>
<span data-ttu-id="e1c3d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1c3d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



