---
title: remoteAssistancePartner aktualisieren
description: Aktualisieren der Eigenschaften eines remoteAssistancePartner-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7799108ed97e14da16a3e8fbfee9642f9980891c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251902"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="54630-103">remoteAssistancePartner aktualisieren</span><span class="sxs-lookup"><span data-stu-id="54630-103">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="54630-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="54630-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54630-105">Aktualisieren der Eigenschaften eines [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="54630-105">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54630-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="54630-106">Prerequisites</span></span>
<span data-ttu-id="54630-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="54630-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="54630-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="54630-109">Permission type</span></span>|<span data-ttu-id="54630-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="54630-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54630-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="54630-111">Delegated (work or school account)</span></span>|<span data-ttu-id="54630-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54630-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="54630-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="54630-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54630-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54630-114">Not supported.</span></span>|
|<span data-ttu-id="54630-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="54630-115">Application</span></span>|<span data-ttu-id="54630-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54630-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54630-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="54630-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="54630-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="54630-118">Request headers</span></span>
|<span data-ttu-id="54630-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="54630-119">Header</span></span>|<span data-ttu-id="54630-120">Wert</span><span class="sxs-lookup"><span data-stu-id="54630-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54630-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="54630-121">Authorization</span></span>|<span data-ttu-id="54630-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="54630-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54630-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="54630-123">Accept</span></span>|<span data-ttu-id="54630-124">application/json</span><span class="sxs-lookup"><span data-stu-id="54630-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54630-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="54630-125">Request body</span></span>
<span data-ttu-id="54630-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="54630-126">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="54630-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="54630-127">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="54630-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="54630-128">Property</span></span>|<span data-ttu-id="54630-129">Typ</span><span class="sxs-lookup"><span data-stu-id="54630-129">Type</span></span>|<span data-ttu-id="54630-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54630-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54630-131">id</span><span class="sxs-lookup"><span data-stu-id="54630-131">id</span></span>|<span data-ttu-id="54630-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54630-132">String</span></span>|<span data-ttu-id="54630-133">Der eindeutige Bezeichner des Partners.</span><span class="sxs-lookup"><span data-stu-id="54630-133">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="54630-134">displayName</span><span class="sxs-lookup"><span data-stu-id="54630-134">displayName</span></span>|<span data-ttu-id="54630-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54630-135">String</span></span>|<span data-ttu-id="54630-136">Der Anzeigename des Partners.</span><span class="sxs-lookup"><span data-stu-id="54630-136">Display name of the partner.</span></span>|
|<span data-ttu-id="54630-137">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="54630-137">onboardingUrl</span></span>|<span data-ttu-id="54630-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54630-138">String</span></span>|<span data-ttu-id="54630-139">Die URL des Onboarding-Portals des Partners, in dem ein Administrator den Remoteunterstützungsdienst konfigurieren kann.</span><span class="sxs-lookup"><span data-stu-id="54630-139">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="54630-140">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="54630-140">onboardingStatus</span></span>|[<span data-ttu-id="54630-141">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="54630-141">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="54630-142">TBD.</span><span class="sxs-lookup"><span data-stu-id="54630-142">TBD.</span></span> <span data-ttu-id="54630-143">Mögliche Werte sind: `notOnboarded`, `onboarding` und `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="54630-143">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="54630-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="54630-144">lastConnectionDateTime</span></span>|<span data-ttu-id="54630-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54630-145">DateTimeOffset</span></span>|<span data-ttu-id="54630-146">Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung</span><span class="sxs-lookup"><span data-stu-id="54630-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="54630-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="54630-147">Response</span></span>
<span data-ttu-id="54630-148">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="54630-148">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54630-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="54630-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="54630-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="54630-150">Request</span></span>
<span data-ttu-id="54630-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="54630-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
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

### <a name="response"></a><span data-ttu-id="54630-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="54630-152">Response</span></span>
<span data-ttu-id="54630-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="54630-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



