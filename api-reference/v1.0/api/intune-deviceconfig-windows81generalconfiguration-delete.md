---
title: windows81GeneralConfiguration löschen
description: Löscht eine windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da63317ffad50316d88a3a14da0b6c9ac357ecd5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982441"
---
# <a name="delete-windows81generalconfiguration"></a><span data-ttu-id="b7895-103">windows81GeneralConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="b7895-103">Delete windows81GeneralConfiguration</span></span>

> <span data-ttu-id="b7895-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b7895-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7895-105">Löscht eine [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7895-105">Deletes a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7895-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b7895-106">Prerequisites</span></span>
<span data-ttu-id="b7895-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7895-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7895-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b7895-109">Permission type</span></span>|<span data-ttu-id="b7895-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b7895-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7895-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b7895-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b7895-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7895-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b7895-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b7895-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7895-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b7895-114">Not supported.</span></span>|
|<span data-ttu-id="b7895-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b7895-115">Application</span></span>|<span data-ttu-id="b7895-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b7895-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7895-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7895-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b7895-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b7895-118">Request headers</span></span>
|<span data-ttu-id="b7895-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b7895-119">Header</span></span>|<span data-ttu-id="b7895-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b7895-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7895-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7895-121">Authorization</span></span>|<span data-ttu-id="b7895-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b7895-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7895-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b7895-123">Accept</span></span>|<span data-ttu-id="b7895-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b7895-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7895-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b7895-125">Request body</span></span>
<span data-ttu-id="b7895-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b7895-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7895-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7895-127">Response</span></span>
<span data-ttu-id="b7895-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b7895-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b7895-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b7895-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7895-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7895-130">Request</span></span>
<span data-ttu-id="b7895-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b7895-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b7895-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7895-132">Response</span></span>
<span data-ttu-id="b7895-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b7895-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



