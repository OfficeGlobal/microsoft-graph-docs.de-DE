---
title: remoteAssistancePartner aktualisieren
description: Aktualisieren der Eigenschaften eines remoteAssistancePartner-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3b662bd25f42dfe2376af5b4e13ca64771c00bbb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933407"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="1530d-103">remoteAssistancePartner aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1530d-103">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="1530d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1530d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1530d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1530d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1530d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1530d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1530d-107">Aktualisieren der Eigenschaften eines [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1530d-107">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1530d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1530d-108">Prerequisites</span></span>
<span data-ttu-id="1530d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1530d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1530d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1530d-111">Permission type</span></span>|<span data-ttu-id="1530d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1530d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1530d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1530d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1530d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1530d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1530d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1530d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1530d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1530d-116">Not supported.</span></span>|
|<span data-ttu-id="1530d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1530d-117">Application</span></span>|<span data-ttu-id="1530d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1530d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1530d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1530d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="1530d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1530d-120">Request headers</span></span>
|<span data-ttu-id="1530d-121">Header</span><span class="sxs-lookup"><span data-stu-id="1530d-121">Header</span></span>|<span data-ttu-id="1530d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1530d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1530d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1530d-123">Authorization</span></span>|<span data-ttu-id="1530d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1530d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1530d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1530d-125">Accept</span></span>|<span data-ttu-id="1530d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1530d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1530d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1530d-127">Request body</span></span>
<span data-ttu-id="1530d-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="1530d-128">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="1530d-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1530d-129">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="1530d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1530d-130">Property</span></span>|<span data-ttu-id="1530d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1530d-131">Type</span></span>|<span data-ttu-id="1530d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1530d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1530d-133">id</span><span class="sxs-lookup"><span data-stu-id="1530d-133">id</span></span>|<span data-ttu-id="1530d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1530d-134">String</span></span>|<span data-ttu-id="1530d-135">Der eindeutige Bezeichner des Partners.</span><span class="sxs-lookup"><span data-stu-id="1530d-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="1530d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1530d-136">displayName</span></span>|<span data-ttu-id="1530d-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1530d-137">String</span></span>|<span data-ttu-id="1530d-138">Der Anzeigename des Partners.</span><span class="sxs-lookup"><span data-stu-id="1530d-138">Display name of the partner.</span></span>|
|<span data-ttu-id="1530d-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="1530d-139">onboardingUrl</span></span>|<span data-ttu-id="1530d-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1530d-140">String</span></span>|<span data-ttu-id="1530d-141">Die URL des Onboarding-Portals des Partners, in dem ein Administrator den Remoteunterstützungsdienst konfigurieren kann.</span><span class="sxs-lookup"><span data-stu-id="1530d-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="1530d-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="1530d-142">onboardingStatus</span></span>|[<span data-ttu-id="1530d-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="1530d-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="1530d-144">TBD.</span><span class="sxs-lookup"><span data-stu-id="1530d-144">TBD.</span></span> <span data-ttu-id="1530d-145">Mögliche Werte sind: `notOnboarded`, `onboarding` und `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="1530d-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="1530d-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="1530d-146">lastConnectionDateTime</span></span>|<span data-ttu-id="1530d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1530d-147">DateTimeOffset</span></span>|<span data-ttu-id="1530d-148">Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung</span><span class="sxs-lookup"><span data-stu-id="1530d-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="1530d-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="1530d-149">Response</span></span>
<span data-ttu-id="1530d-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1530d-150">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1530d-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1530d-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="1530d-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1530d-152">Request</span></span>
<span data-ttu-id="1530d-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1530d-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
Content-type: application/json
Content-length: 204

{
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="1530d-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="1530d-154">Response</span></span>
<span data-ttu-id="1530d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1530d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





