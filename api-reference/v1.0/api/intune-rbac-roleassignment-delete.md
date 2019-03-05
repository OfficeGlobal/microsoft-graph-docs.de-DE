---
title: roleAssignment löschen
description: Löscht ein roleAssignment-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b90b23f1eb15e37ce0758353f5a1e7fb258fba1
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251300"
---
# <a name="delete-roleassignment"></a><span data-ttu-id="66305-103">roleAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="66305-103">Delete roleAssignment</span></span>

> <span data-ttu-id="66305-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="66305-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66305-105">Löscht ein [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="66305-105">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66305-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="66305-106">Prerequisites</span></span>
<span data-ttu-id="66305-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="66305-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="66305-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="66305-109">Permission type</span></span>|<span data-ttu-id="66305-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="66305-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66305-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="66305-111">Delegated (work or school account)</span></span>|<span data-ttu-id="66305-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66305-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="66305-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="66305-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66305-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66305-114">Not supported.</span></span>|
|<span data-ttu-id="66305-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="66305-115">Application</span></span>|<span data-ttu-id="66305-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66305-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66305-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="66305-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="66305-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="66305-118">Request headers</span></span>
|<span data-ttu-id="66305-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="66305-119">Header</span></span>|<span data-ttu-id="66305-120">Wert</span><span class="sxs-lookup"><span data-stu-id="66305-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66305-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="66305-121">Authorization</span></span>|<span data-ttu-id="66305-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="66305-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66305-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="66305-123">Accept</span></span>|<span data-ttu-id="66305-124">application/json</span><span class="sxs-lookup"><span data-stu-id="66305-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66305-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="66305-125">Request body</span></span>
<span data-ttu-id="66305-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="66305-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66305-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="66305-127">Response</span></span>
<span data-ttu-id="66305-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="66305-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="66305-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="66305-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="66305-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="66305-130">Request</span></span>
<span data-ttu-id="66305-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="66305-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="66305-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="66305-132">Response</span></span>
<span data-ttu-id="66305-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="66305-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



