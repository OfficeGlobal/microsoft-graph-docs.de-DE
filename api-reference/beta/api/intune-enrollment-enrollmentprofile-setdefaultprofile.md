---
title: setDefaultProfile-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: db1ab2e894ea80d0b32ecc4f726ee9a43d94818a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141671"
---
# <a name="setdefaultprofile-action"></a><span data-ttu-id="b7d62-103">setDefaultProfile-Aktion</span><span class="sxs-lookup"><span data-stu-id="b7d62-103">setDefaultProfile action</span></span>

> <span data-ttu-id="b7d62-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b7d62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7d62-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b7d62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7d62-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b7d62-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7d62-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b7d62-107">Prerequisites</span></span>
<span data-ttu-id="b7d62-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b7d62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b7d62-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b7d62-110">Permission type</span></span>|<span data-ttu-id="b7d62-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b7d62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7d62-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b7d62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7d62-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7d62-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b7d62-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b7d62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7d62-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b7d62-115">Not supported.</span></span>|
|<span data-ttu-id="b7d62-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b7d62-116">Application</span></span>|<span data-ttu-id="b7d62-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b7d62-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7d62-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7d62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/setDefaultProfile
```

## <a name="request-headers"></a><span data-ttu-id="b7d62-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b7d62-119">Request headers</span></span>
|<span data-ttu-id="b7d62-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b7d62-120">Header</span></span>|<span data-ttu-id="b7d62-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b7d62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7d62-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7d62-122">Authorization</span></span>|<span data-ttu-id="b7d62-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b7d62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7d62-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b7d62-124">Accept</span></span>|<span data-ttu-id="b7d62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7d62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7d62-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b7d62-126">Request body</span></span>
<span data-ttu-id="b7d62-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b7d62-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7d62-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7d62-128">Response</span></span>
<span data-ttu-id="b7d62-129">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="b7d62-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b7d62-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b7d62-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7d62-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7d62-131">Request</span></span>
<span data-ttu-id="b7d62-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b7d62-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/setDefaultProfile
```

### <a name="response"></a><span data-ttu-id="b7d62-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7d62-133">Response</span></span>
<span data-ttu-id="b7d62-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b7d62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




