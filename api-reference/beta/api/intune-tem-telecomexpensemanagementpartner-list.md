---
title: telecomExpenseManagementPartners auflisten
description: Auflisten von Eigenschaften und Beziehungen der telecomExpenseManagementPartner-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 892b91287ce397d5b1a13c679172bdb17e597e1a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968798"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="1abb8-103">telecomExpenseManagementPartners auflisten</span><span class="sxs-lookup"><span data-stu-id="1abb8-103">List telecomExpenseManagementPartners</span></span>

> <span data-ttu-id="1abb8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1abb8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1abb8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1abb8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1abb8-106">Auflisten von Eigenschaften und Beziehungen der [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="1abb8-106">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1abb8-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1abb8-107">Prerequisites</span></span>
<span data-ttu-id="1abb8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1abb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1abb8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1abb8-110">Permission type</span></span>|<span data-ttu-id="1abb8-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1abb8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1abb8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1abb8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1abb8-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1abb8-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1abb8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1abb8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1abb8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1abb8-115">Not supported.</span></span>|
|<span data-ttu-id="1abb8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1abb8-116">Application</span></span>|<span data-ttu-id="1abb8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1abb8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1abb8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1abb8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="1abb8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1abb8-119">Request headers</span></span>
|<span data-ttu-id="1abb8-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1abb8-120">Header</span></span>|<span data-ttu-id="1abb8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1abb8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1abb8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1abb8-122">Authorization</span></span>|<span data-ttu-id="1abb8-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1abb8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1abb8-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1abb8-124">Accept</span></span>|<span data-ttu-id="1abb8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1abb8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1abb8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1abb8-126">Request body</span></span>
<span data-ttu-id="1abb8-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1abb8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1abb8-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="1abb8-128">Response</span></span>
<span data-ttu-id="1abb8-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von Objekten des Typs [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1abb8-129">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1abb8-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1abb8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1abb8-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1abb8-131">Request</span></span>
<span data-ttu-id="1abb8-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1abb8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="1abb8-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="1abb8-133">Response</span></span>
<span data-ttu-id="1abb8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1abb8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 358

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
      "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
      "displayName": "Display Name value",
      "url": "Url value",
      "appAuthorized": true,
      "enabled": true,
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
    }
  ]
}
```




