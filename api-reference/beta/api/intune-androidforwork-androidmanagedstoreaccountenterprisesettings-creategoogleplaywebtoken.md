---
title: createGooglePlayWebToken-Aktion
description: Generiert ein webtoken, das in einer einbettbaren Komponente verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 50355af2e5f9e593501094c0bfd1638cb070df9d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141244"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="6fa68-103">createGooglePlayWebToken-Aktion</span><span class="sxs-lookup"><span data-stu-id="6fa68-103">createGooglePlayWebToken action</span></span>

> <span data-ttu-id="6fa68-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6fa68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fa68-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6fa68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fa68-106">Generiert ein webtoken, das in einer einbettbaren Komponente verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="6fa68-106">Generates a web token that is used in an embeddable component.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fa68-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6fa68-107">Prerequisites</span></span>
<span data-ttu-id="6fa68-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6fa68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6fa68-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6fa68-110">Permission type</span></span>|<span data-ttu-id="6fa68-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6fa68-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fa68-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6fa68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6fa68-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fa68-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6fa68-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6fa68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fa68-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6fa68-115">Not supported.</span></span>|
|<span data-ttu-id="6fa68-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6fa68-116">Application</span></span>|<span data-ttu-id="6fa68-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6fa68-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fa68-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6fa68-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="6fa68-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6fa68-119">Request headers</span></span>
|<span data-ttu-id="6fa68-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6fa68-120">Header</span></span>|<span data-ttu-id="6fa68-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6fa68-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fa68-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fa68-122">Authorization</span></span>|<span data-ttu-id="6fa68-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6fa68-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fa68-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6fa68-124">Accept</span></span>|<span data-ttu-id="6fa68-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6fa68-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fa68-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6fa68-126">Request body</span></span>
<span data-ttu-id="6fa68-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="6fa68-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6fa68-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="6fa68-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6fa68-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6fa68-129">Property</span></span>|<span data-ttu-id="6fa68-130">Typ</span><span class="sxs-lookup"><span data-stu-id="6fa68-130">Type</span></span>|<span data-ttu-id="6fa68-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6fa68-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fa68-132">parentUri</span><span class="sxs-lookup"><span data-stu-id="6fa68-132">parentUri</span></span>|<span data-ttu-id="6fa68-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6fa68-133">String</span></span>|<span data-ttu-id="6fa68-134">Der HTTPS-Pfad der Seite, die die Komponente hostet.</span><span class="sxs-lookup"><span data-stu-id="6fa68-134">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="6fa68-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="6fa68-135">Response</span></span>
<span data-ttu-id="6fa68-136">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6fa68-136">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fa68-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6fa68-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fa68-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6fa68-138">Request</span></span>
<span data-ttu-id="6fa68-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6fa68-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="6fa68-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="6fa68-140">Response</span></span>
<span data-ttu-id="6fa68-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6fa68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```




