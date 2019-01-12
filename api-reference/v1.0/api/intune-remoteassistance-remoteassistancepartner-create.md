---
title: remoteAssistancePartner erstellen
description: Erstellen eines neuen RemoteAssistancePartner-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a9081af7c6bc79540eb0a1593f0645771346f539
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951565"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="94c14-103">remoteAssistancePartner erstellen</span><span class="sxs-lookup"><span data-stu-id="94c14-103">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="94c14-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="94c14-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94c14-105">Erstellen eines neuen [RemoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="94c14-105">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="94c14-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="94c14-106">Prerequisites</span></span>
<span data-ttu-id="94c14-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94c14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94c14-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="94c14-109">Permission type</span></span>|<span data-ttu-id="94c14-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="94c14-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94c14-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="94c14-111">Delegated (work or school account)</span></span>|<span data-ttu-id="94c14-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94c14-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="94c14-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="94c14-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94c14-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94c14-114">Not supported.</span></span>|
|<span data-ttu-id="94c14-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="94c14-115">Application</span></span>|<span data-ttu-id="94c14-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94c14-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94c14-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="94c14-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="94c14-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="94c14-118">Request headers</span></span>
|<span data-ttu-id="94c14-119">Header</span><span class="sxs-lookup"><span data-stu-id="94c14-119">Header</span></span>|<span data-ttu-id="94c14-120">Wert</span><span class="sxs-lookup"><span data-stu-id="94c14-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94c14-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="94c14-121">Authorization</span></span>|<span data-ttu-id="94c14-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="94c14-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94c14-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="94c14-123">Accept</span></span>|<span data-ttu-id="94c14-124">application/json</span><span class="sxs-lookup"><span data-stu-id="94c14-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94c14-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="94c14-125">Request body</span></span>
<span data-ttu-id="94c14-126">Geben Sie im Anforderungstext eine JSON-Darstellung des remoteAssistancePartner-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="94c14-126">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="94c14-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des remoteAssistancePartner erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="94c14-127">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="94c14-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="94c14-128">Property</span></span>|<span data-ttu-id="94c14-129">Typ</span><span class="sxs-lookup"><span data-stu-id="94c14-129">Type</span></span>|<span data-ttu-id="94c14-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94c14-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94c14-131">id</span><span class="sxs-lookup"><span data-stu-id="94c14-131">id</span></span>|<span data-ttu-id="94c14-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="94c14-132">String</span></span>|<span data-ttu-id="94c14-133">Der eindeutige Bezeichner des Partners.</span><span class="sxs-lookup"><span data-stu-id="94c14-133">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="94c14-134">displayName</span><span class="sxs-lookup"><span data-stu-id="94c14-134">displayName</span></span>|<span data-ttu-id="94c14-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="94c14-135">String</span></span>|<span data-ttu-id="94c14-136">Der Anzeigename des Partners.</span><span class="sxs-lookup"><span data-stu-id="94c14-136">Display name of the partner.</span></span>|
|<span data-ttu-id="94c14-137">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="94c14-137">onboardingUrl</span></span>|<span data-ttu-id="94c14-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="94c14-138">String</span></span>|<span data-ttu-id="94c14-139">Die URL des Onboarding-Portals des Partners, in dem ein Administrator den Remoteunterstützungsdienst konfigurieren kann.</span><span class="sxs-lookup"><span data-stu-id="94c14-139">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="94c14-140">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="94c14-140">onboardingStatus</span></span>|[<span data-ttu-id="94c14-141">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="94c14-141">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="94c14-142">TBD.</span><span class="sxs-lookup"><span data-stu-id="94c14-142">TBD.</span></span> <span data-ttu-id="94c14-143">Mögliche Werte sind: `notOnboarded`, `onboarding` und `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="94c14-143">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="94c14-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="94c14-144">lastConnectionDateTime</span></span>|<span data-ttu-id="94c14-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94c14-145">DateTimeOffset</span></span>|<span data-ttu-id="94c14-146">Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung</span><span class="sxs-lookup"><span data-stu-id="94c14-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="94c14-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="94c14-147">Response</span></span>
<span data-ttu-id="94c14-148">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="94c14-148">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94c14-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="94c14-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="94c14-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="94c14-150">Request</span></span>
<span data-ttu-id="94c14-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="94c14-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="94c14-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="94c14-152">Response</span></span>
<span data-ttu-id="94c14-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="94c14-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```



