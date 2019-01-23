---
title: syncMicrosoftStoreForBusinessApps-Aktion
description: Synchronisiert Intune-Konten mit dem Microsoft Store für Unternehmen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 18a88ef3979cbcaccf41beba1c0870870b46bc57
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415873"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="b636f-103">syncMicrosoftStoreForBusinessApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="b636f-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="b636f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b636f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b636f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b636f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b636f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b636f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b636f-107">Synchronisiert Intune-Konten mit dem Microsoft Store für Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="b636f-107">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b636f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b636f-108">Prerequisites</span></span>
<span data-ttu-id="b636f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b636f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b636f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b636f-111">Permission type</span></span>|<span data-ttu-id="b636f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b636f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b636f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b636f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b636f-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="b636f-114">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="b636f-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b636f-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b636f-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b636f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b636f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b636f-117">Not supported.</span></span>|
|<span data-ttu-id="b636f-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b636f-118">Application</span></span>|<span data-ttu-id="b636f-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b636f-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b636f-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b636f-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="b636f-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b636f-121">Request headers</span></span>
|<span data-ttu-id="b636f-122">Header</span><span class="sxs-lookup"><span data-stu-id="b636f-122">Header</span></span>|<span data-ttu-id="b636f-123">Wert</span><span class="sxs-lookup"><span data-stu-id="b636f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b636f-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b636f-124">Authorization</span></span>|<span data-ttu-id="b636f-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b636f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b636f-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b636f-126">Accept</span></span>|<span data-ttu-id="b636f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b636f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b636f-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b636f-128">Request body</span></span>
<span data-ttu-id="b636f-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b636f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b636f-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="b636f-130">Response</span></span>
<span data-ttu-id="b636f-131">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="b636f-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b636f-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b636f-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="b636f-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b636f-133">Request</span></span>
<span data-ttu-id="b636f-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b636f-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="b636f-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="b636f-135">Response</span></span>
<span data-ttu-id="b636f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b636f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



