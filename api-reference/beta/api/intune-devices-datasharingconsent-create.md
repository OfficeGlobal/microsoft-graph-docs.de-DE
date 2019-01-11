---
title: Erstellen von dataSharingConsent
description: Erstellen eines neuen DataSharingConsent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cf45db12a9876d9be89d20fa3328e89eeea82013
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862286"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="dd920-103">Erstellen von dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="dd920-103">Create dataSharingConsent</span></span>

> <span data-ttu-id="dd920-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dd920-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd920-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd920-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd920-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dd920-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd920-107">Erstellen eines neuen [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="dd920-107">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd920-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dd920-108">Prerequisites</span></span>
<span data-ttu-id="dd920-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd920-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd920-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd920-111">Permission type</span></span>|<span data-ttu-id="dd920-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd920-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd920-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd920-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd920-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd920-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dd920-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd920-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd920-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd920-116">Not supported.</span></span>|
|<span data-ttu-id="dd920-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd920-117">Application</span></span>|<span data-ttu-id="dd920-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd920-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd920-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd920-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="dd920-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd920-120">Request headers</span></span>
|<span data-ttu-id="dd920-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dd920-121">Header</span></span>|<span data-ttu-id="dd920-122">Wert</span><span class="sxs-lookup"><span data-stu-id="dd920-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd920-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd920-123">Authorization</span></span>|<span data-ttu-id="dd920-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dd920-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd920-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dd920-125">Accept</span></span>|<span data-ttu-id="dd920-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd920-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd920-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd920-127">Request body</span></span>
<span data-ttu-id="dd920-128">Geben Sie im Textkörper Anforderung für das Objekt DataSharingConsent eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="dd920-128">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="dd920-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DataSharingConsent erstellen.</span><span class="sxs-lookup"><span data-stu-id="dd920-129">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="dd920-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dd920-130">Property</span></span>|<span data-ttu-id="dd920-131">Typ</span><span class="sxs-lookup"><span data-stu-id="dd920-131">Type</span></span>|<span data-ttu-id="dd920-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd920-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd920-133">id</span><span class="sxs-lookup"><span data-stu-id="dd920-133">id</span></span>|<span data-ttu-id="dd920-134">String</span><span class="sxs-lookup"><span data-stu-id="dd920-134">String</span></span>|<span data-ttu-id="dd920-135">Die Daten sharing Zustimmung Id</span><span class="sxs-lookup"><span data-stu-id="dd920-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="dd920-136">von Ihnen eingegebene Dienstanzeigename</span><span class="sxs-lookup"><span data-stu-id="dd920-136">serviceDisplayName</span></span>|<span data-ttu-id="dd920-137">String</span><span class="sxs-lookup"><span data-stu-id="dd920-137">String</span></span>|<span data-ttu-id="dd920-138">Der Anzeigename der Dienst Workflow</span><span class="sxs-lookup"><span data-stu-id="dd920-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="dd920-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="dd920-139">termsUrl</span></span>|<span data-ttu-id="dd920-140">String</span><span class="sxs-lookup"><span data-stu-id="dd920-140">String</span></span>|<span data-ttu-id="dd920-141">Die TermsUrl für die Datenfreigabe Zustimmung</span><span class="sxs-lookup"><span data-stu-id="dd920-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="dd920-142">erteilt</span><span class="sxs-lookup"><span data-stu-id="dd920-142">granted</span></span>|<span data-ttu-id="dd920-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd920-143">Boolean</span></span>|<span data-ttu-id="dd920-144">Den gewährten Status für die Datenfreigabe Zustimmung</span><span class="sxs-lookup"><span data-stu-id="dd920-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="dd920-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="dd920-145">grantDateTime</span></span>|<span data-ttu-id="dd920-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd920-146">DateTimeOffset</span></span>|<span data-ttu-id="dd920-147">Die Zeit Zustimmung wurde für dieses Konto erteilt.</span><span class="sxs-lookup"><span data-stu-id="dd920-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="dd920-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="dd920-148">grantedByUpn</span></span>|<span data-ttu-id="dd920-149">String</span><span class="sxs-lookup"><span data-stu-id="dd920-149">String</span></span>|<span data-ttu-id="dd920-150">Den Upn des Benutzers, der für dieses Konto Zustimmung eingeholt</span><span class="sxs-lookup"><span data-stu-id="dd920-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="dd920-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="dd920-151">grantedByUserId</span></span>|<span data-ttu-id="dd920-152">String</span><span class="sxs-lookup"><span data-stu-id="dd920-152">String</span></span>|<span data-ttu-id="dd920-153">Die Benutzer-ID des Benutzers, der für dieses Konto Zustimmung eingeholt</span><span class="sxs-lookup"><span data-stu-id="dd920-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="dd920-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd920-154">Response</span></span>
<span data-ttu-id="dd920-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="dd920-155">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd920-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd920-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd920-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd920-157">Request</span></span>
<span data-ttu-id="dd920-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd920-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents
Content-type: application/json
Content-length: 333

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```

### <a name="response"></a><span data-ttu-id="dd920-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd920-159">Response</span></span>
<span data-ttu-id="dd920-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd920-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 382

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "333387f7-87f7-3333-f787-3333f7873333",
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```





