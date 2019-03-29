---
title: enrollmentConfigurationAssignment löschen
description: Löscht ein enrollmentConfigurationAssignment-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 41d06972a05e4cb33db60595054f0c45114df0d7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978892"
---
# <a name="delete-enrollmentconfigurationassignment"></a><span data-ttu-id="53eed-103">enrollmentConfigurationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="53eed-103">Delete enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="53eed-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="53eed-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53eed-105">Löscht ein [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="53eed-105">Deletes a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53eed-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="53eed-106">Prerequisites</span></span>
<span data-ttu-id="53eed-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53eed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53eed-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53eed-109">Permission type</span></span>|<span data-ttu-id="53eed-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53eed-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53eed-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53eed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53eed-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53eed-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="53eed-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53eed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53eed-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53eed-114">Not supported.</span></span>|
|<span data-ttu-id="53eed-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53eed-115">Application</span></span>|<span data-ttu-id="53eed-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53eed-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53eed-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53eed-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="53eed-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53eed-118">Request headers</span></span>
|<span data-ttu-id="53eed-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="53eed-119">Header</span></span>|<span data-ttu-id="53eed-120">Wert</span><span class="sxs-lookup"><span data-stu-id="53eed-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53eed-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53eed-121">Authorization</span></span>|<span data-ttu-id="53eed-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="53eed-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53eed-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="53eed-123">Accept</span></span>|<span data-ttu-id="53eed-124">application/json</span><span class="sxs-lookup"><span data-stu-id="53eed-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53eed-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53eed-125">Request body</span></span>
<span data-ttu-id="53eed-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="53eed-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53eed-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="53eed-127">Response</span></span>
<span data-ttu-id="53eed-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53eed-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="53eed-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53eed-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="53eed-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53eed-130">Request</span></span>
<span data-ttu-id="53eed-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53eed-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="53eed-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="53eed-132">Response</span></span>
<span data-ttu-id="53eed-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53eed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



