---
title: DepMacOSEnrollmentProfile löschen
description: Löscht eine DepMacOSEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 209d48fee1b4b8451b14654f8652844c76930f8a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411904"
---
# <a name="delete-depmacosenrollmentprofile"></a><span data-ttu-id="76507-103">DepMacOSEnrollmentProfile löschen</span><span class="sxs-lookup"><span data-stu-id="76507-103">Delete depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="76507-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="76507-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="76507-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="76507-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="76507-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="76507-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76507-107">Löscht eine [DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="76507-107">Deletes a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76507-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="76507-108">Prerequisites</span></span>
<span data-ttu-id="76507-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="76507-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="76507-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="76507-111">Permission type</span></span>|<span data-ttu-id="76507-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="76507-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76507-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="76507-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76507-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76507-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="76507-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="76507-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76507-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76507-116">Not supported.</span></span>|
|<span data-ttu-id="76507-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="76507-117">Application</span></span>|<span data-ttu-id="76507-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76507-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76507-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="76507-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="76507-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="76507-120">Request headers</span></span>
|<span data-ttu-id="76507-121">Header</span><span class="sxs-lookup"><span data-stu-id="76507-121">Header</span></span>|<span data-ttu-id="76507-122">Wert</span><span class="sxs-lookup"><span data-stu-id="76507-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76507-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="76507-123">Authorization</span></span>|<span data-ttu-id="76507-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="76507-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76507-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="76507-125">Accept</span></span>|<span data-ttu-id="76507-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76507-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76507-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="76507-127">Request body</span></span>
<span data-ttu-id="76507-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="76507-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76507-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="76507-129">Response</span></span>
<span data-ttu-id="76507-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76507-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="76507-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="76507-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="76507-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="76507-132">Request</span></span>
<span data-ttu-id="76507-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="76507-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="76507-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="76507-134">Response</span></span>
<span data-ttu-id="76507-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76507-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




