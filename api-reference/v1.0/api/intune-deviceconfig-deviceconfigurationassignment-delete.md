---
title: deviceConfigurationAssignment löschen
description: Löscht ein deviceConfigurationAssignment-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4869eea8a786d805a5c58b9bfdd90a3f6bec9b3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250075"
---
# <a name="delete-deviceconfigurationassignment"></a><span data-ttu-id="ccc01-103">deviceConfigurationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="ccc01-103">Delete deviceConfigurationAssignment</span></span>

> <span data-ttu-id="ccc01-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ccc01-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccc01-105">Löscht ein [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="ccc01-105">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccc01-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ccc01-106">Prerequisites</span></span>
<span data-ttu-id="ccc01-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ccc01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ccc01-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ccc01-109">Permission type</span></span>|<span data-ttu-id="ccc01-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ccc01-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccc01-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ccc01-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ccc01-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccc01-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ccc01-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ccc01-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccc01-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ccc01-114">Not supported.</span></span>|
|<span data-ttu-id="ccc01-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ccc01-115">Application</span></span>|<span data-ttu-id="ccc01-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ccc01-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccc01-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ccc01-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ccc01-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ccc01-118">Request headers</span></span>
|<span data-ttu-id="ccc01-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ccc01-119">Header</span></span>|<span data-ttu-id="ccc01-120">Wert</span><span class="sxs-lookup"><span data-stu-id="ccc01-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccc01-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccc01-121">Authorization</span></span>|<span data-ttu-id="ccc01-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ccc01-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccc01-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ccc01-123">Accept</span></span>|<span data-ttu-id="ccc01-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ccc01-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccc01-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ccc01-125">Request body</span></span>
<span data-ttu-id="ccc01-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ccc01-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccc01-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ccc01-127">Response</span></span>
<span data-ttu-id="ccc01-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ccc01-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ccc01-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ccc01-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccc01-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ccc01-130">Request</span></span>
<span data-ttu-id="ccc01-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ccc01-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="ccc01-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ccc01-132">Response</span></span>
<span data-ttu-id="ccc01-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ccc01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



