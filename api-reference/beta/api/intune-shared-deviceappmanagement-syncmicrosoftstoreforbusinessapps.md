---
title: syncMicrosoftStoreForBusinessApps-Aktion
description: Synchronisiert Intune-Konten mit dem Microsoft Store für Unternehmen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 18a88ef3979cbcaccf41beba1c0870870b46bc57
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969995"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="39612-103">syncMicrosoftStoreForBusinessApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="39612-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="39612-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="39612-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="39612-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="39612-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39612-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="39612-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39612-107">Synchronisiert Intune-Konten mit dem Microsoft Store für Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="39612-107">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39612-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="39612-108">Prerequisites</span></span>
<span data-ttu-id="39612-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39612-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39612-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="39612-111">Permission type</span></span>|<span data-ttu-id="39612-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="39612-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39612-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="39612-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="39612-114">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="39612-114">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="39612-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39612-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="39612-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="39612-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39612-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39612-117">Not supported.</span></span>|
|<span data-ttu-id="39612-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="39612-118">Application</span></span>|<span data-ttu-id="39612-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39612-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39612-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39612-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="39612-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39612-121">Request headers</span></span>
|<span data-ttu-id="39612-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="39612-122">Header</span></span>|<span data-ttu-id="39612-123">Wert</span><span class="sxs-lookup"><span data-stu-id="39612-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39612-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="39612-124">Authorization</span></span>|<span data-ttu-id="39612-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="39612-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39612-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="39612-126">Accept</span></span>|<span data-ttu-id="39612-127">application/json</span><span class="sxs-lookup"><span data-stu-id="39612-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39612-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="39612-128">Request body</span></span>
<span data-ttu-id="39612-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="39612-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39612-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="39612-130">Response</span></span>
<span data-ttu-id="39612-131">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39612-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="39612-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="39612-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="39612-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39612-133">Request</span></span>
<span data-ttu-id="39612-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39612-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="39612-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="39612-135">Response</span></span>
<span data-ttu-id="39612-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39612-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



