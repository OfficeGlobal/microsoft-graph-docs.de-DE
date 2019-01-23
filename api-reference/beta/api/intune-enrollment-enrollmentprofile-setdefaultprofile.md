---
title: SetDefaultProfile Aktion
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4087cfdf9e84fd62f6f1ba039506b1901d6989f9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413626"
---
# <a name="setdefaultprofile-action"></a><span data-ttu-id="cf08b-103">SetDefaultProfile Aktion</span><span class="sxs-lookup"><span data-stu-id="cf08b-103">setDefaultProfile action</span></span>

> <span data-ttu-id="cf08b-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="cf08b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cf08b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cf08b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf08b-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cf08b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf08b-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="cf08b-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf08b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cf08b-108">Prerequisites</span></span>
<span data-ttu-id="cf08b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cf08b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cf08b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf08b-111">Permission type</span></span>|<span data-ttu-id="cf08b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf08b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf08b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf08b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf08b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf08b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cf08b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf08b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf08b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf08b-116">Not supported.</span></span>|
|<span data-ttu-id="cf08b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf08b-117">Application</span></span>|<span data-ttu-id="cf08b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf08b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf08b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf08b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/setDefaultProfile
```

## <a name="request-headers"></a><span data-ttu-id="cf08b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf08b-120">Request headers</span></span>
|<span data-ttu-id="cf08b-121">Header</span><span class="sxs-lookup"><span data-stu-id="cf08b-121">Header</span></span>|<span data-ttu-id="cf08b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="cf08b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf08b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cf08b-123">Authorization</span></span>|<span data-ttu-id="cf08b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cf08b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf08b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cf08b-125">Accept</span></span>|<span data-ttu-id="cf08b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf08b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf08b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf08b-127">Request body</span></span>
<span data-ttu-id="cf08b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cf08b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf08b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf08b-129">Response</span></span>
<span data-ttu-id="cf08b-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="cf08b-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cf08b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf08b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf08b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf08b-132">Request</span></span>
<span data-ttu-id="cf08b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf08b-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/setDefaultProfile
```

### <a name="response"></a><span data-ttu-id="cf08b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf08b-134">Response</span></span>
<span data-ttu-id="cf08b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf08b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




