---
title: remoteAssistancePartner erstellen
description: Erstellen eines neuen RemoteAssistancePartner-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11db25c139f0c1897b65887aa9c428a5069032ef
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973019"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="c65c0-103">remoteAssistancePartner erstellen</span><span class="sxs-lookup"><span data-stu-id="c65c0-103">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="c65c0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c65c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c65c0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c65c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c65c0-106">Erstellen eines neuen [RemoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c65c0-106">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c65c0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c65c0-107">Prerequisites</span></span>
<span data-ttu-id="c65c0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c65c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c65c0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c65c0-110">Permission type</span></span>|<span data-ttu-id="c65c0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c65c0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c65c0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c65c0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c65c0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c65c0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c65c0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c65c0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c65c0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c65c0-115">Not supported.</span></span>|
|<span data-ttu-id="c65c0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c65c0-116">Application</span></span>|<span data-ttu-id="c65c0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c65c0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c65c0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c65c0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="c65c0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c65c0-119">Request headers</span></span>
|<span data-ttu-id="c65c0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c65c0-120">Header</span></span>|<span data-ttu-id="c65c0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c65c0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c65c0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c65c0-122">Authorization</span></span>|<span data-ttu-id="c65c0-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c65c0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c65c0-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c65c0-124">Accept</span></span>|<span data-ttu-id="c65c0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c65c0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c65c0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c65c0-126">Request body</span></span>
<span data-ttu-id="c65c0-127">Geben Sie im Anforderungstext eine JSON-Darstellung des remoteAssistancePartner-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c65c0-127">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="c65c0-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des remoteAssistancePartner erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c65c0-128">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="c65c0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c65c0-129">Property</span></span>|<span data-ttu-id="c65c0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c65c0-130">Type</span></span>|<span data-ttu-id="c65c0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c65c0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c65c0-132">id</span><span class="sxs-lookup"><span data-stu-id="c65c0-132">id</span></span>|<span data-ttu-id="c65c0-133">String</span><span class="sxs-lookup"><span data-stu-id="c65c0-133">String</span></span>|<span data-ttu-id="c65c0-134">Der eindeutige Bezeichner des Partners.</span><span class="sxs-lookup"><span data-stu-id="c65c0-134">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="c65c0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c65c0-135">displayName</span></span>|<span data-ttu-id="c65c0-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c65c0-136">String</span></span>|<span data-ttu-id="c65c0-137">Der Anzeigename des Partners.</span><span class="sxs-lookup"><span data-stu-id="c65c0-137">Display name of the partner.</span></span>|
|<span data-ttu-id="c65c0-138">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="c65c0-138">onboardingUrl</span></span>|<span data-ttu-id="c65c0-139">String</span><span class="sxs-lookup"><span data-stu-id="c65c0-139">String</span></span>|<span data-ttu-id="c65c0-140">Die URL des Onboarding-Portals des Partners, in dem ein Administrator den Remoteunterstützungsdienst konfigurieren kann.</span><span class="sxs-lookup"><span data-stu-id="c65c0-140">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="c65c0-141">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="c65c0-141">onboardingStatus</span></span>|[<span data-ttu-id="c65c0-142">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="c65c0-142">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="c65c0-143">TBD.</span><span class="sxs-lookup"><span data-stu-id="c65c0-143">TBD.</span></span> <span data-ttu-id="c65c0-144">Mögliche Werte sind: `notOnboarded`, `onboarding` und `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="c65c0-144">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="c65c0-145">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="c65c0-145">lastConnectionDateTime</span></span>|<span data-ttu-id="c65c0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c65c0-146">DateTimeOffset</span></span>|<span data-ttu-id="c65c0-147">Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung</span><span class="sxs-lookup"><span data-stu-id="c65c0-147">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="c65c0-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="c65c0-148">Response</span></span>
<span data-ttu-id="c65c0-149">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c65c0-149">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c65c0-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c65c0-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="c65c0-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c65c0-151">Request</span></span>
<span data-ttu-id="c65c0-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c65c0-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners
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

### <a name="response"></a><span data-ttu-id="c65c0-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="c65c0-153">Response</span></span>
<span data-ttu-id="c65c0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c65c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




