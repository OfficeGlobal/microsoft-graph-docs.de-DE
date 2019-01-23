---
title: disconnect-Aktion
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ce32751d7d4d2ad2b00e029bbcaec0e8655e2053
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393914"
---
# <a name="disconnect-action"></a><span data-ttu-id="0ed03-103">disconnect-Aktion</span><span class="sxs-lookup"><span data-stu-id="0ed03-103">disconnect action</span></span>

> <span data-ttu-id="0ed03-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0ed03-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0ed03-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0ed03-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ed03-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0ed03-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ed03-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0ed03-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ed03-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0ed03-108">Prerequisites</span></span>
<span data-ttu-id="0ed03-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0ed03-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0ed03-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0ed03-111">Permission type</span></span>|<span data-ttu-id="0ed03-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0ed03-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ed03-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0ed03-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ed03-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ed03-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0ed03-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0ed03-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ed03-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ed03-116">Not supported.</span></span>|
|<span data-ttu-id="0ed03-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0ed03-117">Application</span></span>|<span data-ttu-id="0ed03-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ed03-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ed03-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ed03-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/disconnect
```

## <a name="request-headers"></a><span data-ttu-id="0ed03-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0ed03-120">Request headers</span></span>
|<span data-ttu-id="0ed03-121">Header</span><span class="sxs-lookup"><span data-stu-id="0ed03-121">Header</span></span>|<span data-ttu-id="0ed03-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0ed03-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ed03-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0ed03-123">Authorization</span></span>|<span data-ttu-id="0ed03-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0ed03-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ed03-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0ed03-125">Accept</span></span>|<span data-ttu-id="0ed03-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ed03-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ed03-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0ed03-127">Request body</span></span>
<span data-ttu-id="0ed03-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0ed03-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ed03-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ed03-129">Response</span></span>
<span data-ttu-id="0ed03-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="0ed03-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0ed03-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0ed03-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ed03-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ed03-132">Request</span></span>
<span data-ttu-id="0ed03-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0ed03-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/disconnect
```

### <a name="response"></a><span data-ttu-id="0ed03-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ed03-134">Response</span></span>
<span data-ttu-id="0ed03-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0ed03-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




