---
title: UploadDepToken Aktion
description: Lädt ein neues Gerät Registrierung Programm Token hoch
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 98c663b80ecfbc2fb1641b8db8bb48af9215c885
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417049"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="35fc7-103">UploadDepToken Aktion</span><span class="sxs-lookup"><span data-stu-id="35fc7-103">uploadDepToken action</span></span>

> <span data-ttu-id="35fc7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="35fc7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="35fc7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="35fc7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35fc7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="35fc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35fc7-107">Lädt ein neues Gerät Registrierung Programm Token hoch</span><span class="sxs-lookup"><span data-stu-id="35fc7-107">Uploads a new Device Enrollment Program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35fc7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="35fc7-108">Prerequisites</span></span>
<span data-ttu-id="35fc7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="35fc7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="35fc7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="35fc7-111">Permission type</span></span>|<span data-ttu-id="35fc7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="35fc7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35fc7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="35fc7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35fc7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35fc7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="35fc7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="35fc7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35fc7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35fc7-116">Not supported.</span></span>|
|<span data-ttu-id="35fc7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="35fc7-117">Application</span></span>|<span data-ttu-id="35fc7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35fc7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35fc7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="35fc7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="35fc7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="35fc7-120">Request headers</span></span>
|<span data-ttu-id="35fc7-121">Header</span><span class="sxs-lookup"><span data-stu-id="35fc7-121">Header</span></span>|<span data-ttu-id="35fc7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="35fc7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35fc7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="35fc7-123">Authorization</span></span>|<span data-ttu-id="35fc7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="35fc7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35fc7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="35fc7-125">Accept</span></span>|<span data-ttu-id="35fc7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35fc7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35fc7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="35fc7-127">Request body</span></span>
<span data-ttu-id="35fc7-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="35fc7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="35fc7-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="35fc7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="35fc7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="35fc7-130">Property</span></span>|<span data-ttu-id="35fc7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="35fc7-131">Type</span></span>|<span data-ttu-id="35fc7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35fc7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35fc7-133">appleId</span><span class="sxs-lookup"><span data-stu-id="35fc7-133">appleId</span></span>|<span data-ttu-id="35fc7-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="35fc7-134">String</span></span>|<span data-ttu-id="35fc7-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="35fc7-135">Not yet documented</span></span>|
|<span data-ttu-id="35fc7-136">depToken</span><span class="sxs-lookup"><span data-stu-id="35fc7-136">depToken</span></span>|<span data-ttu-id="35fc7-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="35fc7-137">String</span></span>|<span data-ttu-id="35fc7-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="35fc7-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="35fc7-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="35fc7-139">Response</span></span>
<span data-ttu-id="35fc7-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="35fc7-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="35fc7-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="35fc7-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="35fc7-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="35fc7-142">Request</span></span>
<span data-ttu-id="35fc7-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="35fc7-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="35fc7-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="35fc7-144">Response</span></span>
<span data-ttu-id="35fc7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="35fc7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




