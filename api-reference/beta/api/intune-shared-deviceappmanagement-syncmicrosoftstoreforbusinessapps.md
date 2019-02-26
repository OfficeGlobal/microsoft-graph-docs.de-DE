---
title: syncMicrosoftStoreForBusinessApps-Aktion
description: Synchronisiert Intune-Konten mit dem Microsoft Store für Unternehmen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ab2f623754e40db39f649aab562fd2f480e63684
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148839"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="7e082-103">syncMicrosoftStoreForBusinessApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="7e082-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="7e082-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="7e082-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7e082-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7e082-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e082-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7e082-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e082-107">Synchronisiert Intune-Konten mit dem Microsoft Store für Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="7e082-107">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e082-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7e082-108">Prerequisites</span></span>
<span data-ttu-id="7e082-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e082-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="7e082-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7e082-111">Permission type</span></span>|<span data-ttu-id="7e082-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7e082-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e082-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7e082-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7e082-114">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="7e082-114">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="7e082-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e082-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7e082-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7e082-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e082-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e082-117">Not supported.</span></span>|
|<span data-ttu-id="7e082-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7e082-118">Application</span></span>|<span data-ttu-id="7e082-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e082-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e082-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e082-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="7e082-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7e082-121">Request headers</span></span>
|<span data-ttu-id="7e082-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7e082-122">Header</span></span>|<span data-ttu-id="7e082-123">Wert</span><span class="sxs-lookup"><span data-stu-id="7e082-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e082-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e082-124">Authorization</span></span>|<span data-ttu-id="7e082-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7e082-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e082-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7e082-126">Accept</span></span>|<span data-ttu-id="7e082-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7e082-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e082-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7e082-128">Request body</span></span>
<span data-ttu-id="7e082-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7e082-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e082-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e082-130">Response</span></span>
<span data-ttu-id="7e082-131">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="7e082-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7e082-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7e082-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="7e082-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e082-133">Request</span></span>
<span data-ttu-id="7e082-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7e082-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="7e082-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e082-135">Response</span></span>
<span data-ttu-id="7e082-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7e082-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



