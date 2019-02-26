---
title: beginOnboarding-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6045eb49c428db548ba104c3c9cb2184d430b35
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254499"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="09f8f-103">beginOnboarding-Aktion</span><span class="sxs-lookup"><span data-stu-id="09f8f-103">beginOnboarding action</span></span>

> <span data-ttu-id="09f8f-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="09f8f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09f8f-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="09f8f-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09f8f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="09f8f-106">Prerequisites</span></span>
<span data-ttu-id="09f8f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="09f8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="09f8f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="09f8f-109">Permission type</span></span>|<span data-ttu-id="09f8f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="09f8f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09f8f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="09f8f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="09f8f-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09f8f-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="09f8f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="09f8f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09f8f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09f8f-114">Not supported.</span></span>|
|<span data-ttu-id="09f8f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="09f8f-115">Application</span></span>|<span data-ttu-id="09f8f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09f8f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09f8f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="09f8f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="09f8f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="09f8f-118">Request headers</span></span>
|<span data-ttu-id="09f8f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="09f8f-119">Header</span></span>|<span data-ttu-id="09f8f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="09f8f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09f8f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="09f8f-121">Authorization</span></span>|<span data-ttu-id="09f8f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="09f8f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09f8f-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="09f8f-123">Accept</span></span>|<span data-ttu-id="09f8f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="09f8f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09f8f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="09f8f-125">Request body</span></span>
<span data-ttu-id="09f8f-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="09f8f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09f8f-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="09f8f-127">Response</span></span>
<span data-ttu-id="09f8f-128">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="09f8f-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="09f8f-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="09f8f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="09f8f-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09f8f-130">Request</span></span>
<span data-ttu-id="09f8f-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="09f8f-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="09f8f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="09f8f-132">Response</span></span>
<span data-ttu-id="09f8f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09f8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



