---
title: remoteAssistancePartner erstellen
description: Erstellen eines neuen RemoteAssistancePartner-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b1f8306c3ece3b5153a9352c38e41eb89e71d6b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410427"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="c302f-103">remoteAssistancePartner erstellen</span><span class="sxs-lookup"><span data-stu-id="c302f-103">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="c302f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c302f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c302f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c302f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c302f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c302f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c302f-107">Erstellen eines neuen [RemoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c302f-107">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c302f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c302f-108">Prerequisites</span></span>
<span data-ttu-id="c302f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c302f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c302f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c302f-111">Permission type</span></span>|<span data-ttu-id="c302f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c302f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c302f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c302f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c302f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c302f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c302f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c302f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c302f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c302f-116">Not supported.</span></span>|
|<span data-ttu-id="c302f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c302f-117">Application</span></span>|<span data-ttu-id="c302f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c302f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c302f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c302f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="c302f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c302f-120">Request headers</span></span>
|<span data-ttu-id="c302f-121">Header</span><span class="sxs-lookup"><span data-stu-id="c302f-121">Header</span></span>|<span data-ttu-id="c302f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c302f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c302f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c302f-123">Authorization</span></span>|<span data-ttu-id="c302f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c302f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c302f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c302f-125">Accept</span></span>|<span data-ttu-id="c302f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c302f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c302f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c302f-127">Request body</span></span>
<span data-ttu-id="c302f-128">Geben Sie im Anforderungstext eine JSON-Darstellung des remoteAssistancePartner-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c302f-128">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="c302f-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des remoteAssistancePartner erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c302f-129">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="c302f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c302f-130">Property</span></span>|<span data-ttu-id="c302f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c302f-131">Type</span></span>|<span data-ttu-id="c302f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c302f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c302f-133">id</span><span class="sxs-lookup"><span data-stu-id="c302f-133">id</span></span>|<span data-ttu-id="c302f-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c302f-134">String</span></span>|<span data-ttu-id="c302f-135">Der eindeutige Bezeichner des Partners.</span><span class="sxs-lookup"><span data-stu-id="c302f-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="c302f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c302f-136">displayName</span></span>|<span data-ttu-id="c302f-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c302f-137">String</span></span>|<span data-ttu-id="c302f-138">Der Anzeigename des Partners.</span><span class="sxs-lookup"><span data-stu-id="c302f-138">Display name of the partner.</span></span>|
|<span data-ttu-id="c302f-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="c302f-139">onboardingUrl</span></span>|<span data-ttu-id="c302f-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c302f-140">String</span></span>|<span data-ttu-id="c302f-141">Die URL des Onboarding-Portals des Partners, in dem ein Administrator den Remoteunterstützungsdienst konfigurieren kann.</span><span class="sxs-lookup"><span data-stu-id="c302f-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="c302f-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="c302f-142">onboardingStatus</span></span>|[<span data-ttu-id="c302f-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="c302f-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="c302f-144">TBD.</span><span class="sxs-lookup"><span data-stu-id="c302f-144">TBD.</span></span> <span data-ttu-id="c302f-145">Mögliche Werte sind: `notOnboarded`, `onboarding` und `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="c302f-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="c302f-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="c302f-146">lastConnectionDateTime</span></span>|<span data-ttu-id="c302f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c302f-147">DateTimeOffset</span></span>|<span data-ttu-id="c302f-148">Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung</span><span class="sxs-lookup"><span data-stu-id="c302f-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="c302f-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="c302f-149">Response</span></span>
<span data-ttu-id="c302f-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c302f-150">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c302f-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c302f-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="c302f-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c302f-152">Request</span></span>
<span data-ttu-id="c302f-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c302f-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c302f-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="c302f-154">Response</span></span>
<span data-ttu-id="c302f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c302f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




