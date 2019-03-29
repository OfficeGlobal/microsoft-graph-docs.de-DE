---
title: DataSharingConsent erstellen
description: Erstellen eines neuen dataSharingConsent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bb20f6e6029e33483d28545bf3f9be56b052a8f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978080"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="f7ea3-103">DataSharingConsent erstellen</span><span class="sxs-lookup"><span data-stu-id="f7ea3-103">Create dataSharingConsent</span></span>

> <span data-ttu-id="f7ea3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f7ea3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7ea3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f7ea3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7ea3-106">Erstellen eines neuen [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f7ea3-106">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7ea3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f7ea3-107">Prerequisites</span></span>
<span data-ttu-id="f7ea3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7ea3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7ea3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f7ea3-110">Permission type</span></span>|<span data-ttu-id="f7ea3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f7ea3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7ea3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f7ea3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7ea3-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7ea3-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f7ea3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f7ea3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7ea3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7ea3-115">Not supported.</span></span>|
|<span data-ttu-id="f7ea3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f7ea3-116">Application</span></span>|<span data-ttu-id="f7ea3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7ea3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7ea3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7ea3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="f7ea3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f7ea3-119">Request headers</span></span>
|<span data-ttu-id="f7ea3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f7ea3-120">Header</span></span>|<span data-ttu-id="f7ea3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f7ea3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7ea3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7ea3-122">Authorization</span></span>|<span data-ttu-id="f7ea3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f7ea3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7ea3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f7ea3-124">Accept</span></span>|<span data-ttu-id="f7ea3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f7ea3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7ea3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f7ea3-126">Request body</span></span>
<span data-ttu-id="f7ea3-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das dataSharingConsent-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="f7ea3-127">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="f7ea3-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der dataSharingConsent erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f7ea3-128">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="f7ea3-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f7ea3-129">Property</span></span>|<span data-ttu-id="f7ea3-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f7ea3-130">Type</span></span>|<span data-ttu-id="f7ea3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7ea3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7ea3-132">id</span><span class="sxs-lookup"><span data-stu-id="f7ea3-132">id</span></span>|<span data-ttu-id="f7ea3-133">String</span><span class="sxs-lookup"><span data-stu-id="f7ea3-133">String</span></span>|<span data-ttu-id="f7ea3-134">Die Einwilligungs-ID für die Datenfreigabe</span><span class="sxs-lookup"><span data-stu-id="f7ea3-134">The data sharing consent Id</span></span>|
|<span data-ttu-id="f7ea3-135">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f7ea3-135">serviceDisplayName</span></span>|<span data-ttu-id="f7ea3-136">String</span><span class="sxs-lookup"><span data-stu-id="f7ea3-136">String</span></span>|<span data-ttu-id="f7ea3-137">Der Anzeigename des Dienst-Arbeitsflusses</span><span class="sxs-lookup"><span data-stu-id="f7ea3-137">The display name of the service work flow</span></span>|
|<span data-ttu-id="f7ea3-138">termsUrl</span><span class="sxs-lookup"><span data-stu-id="f7ea3-138">termsUrl</span></span>|<span data-ttu-id="f7ea3-139">String</span><span class="sxs-lookup"><span data-stu-id="f7ea3-139">String</span></span>|<span data-ttu-id="f7ea3-140">Die TermsUrl für die Einwilligung zur Datenfreigabe</span><span class="sxs-lookup"><span data-stu-id="f7ea3-140">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="f7ea3-141">granted</span><span class="sxs-lookup"><span data-stu-id="f7ea3-141">granted</span></span>|<span data-ttu-id="f7ea3-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f7ea3-142">Boolean</span></span>|<span data-ttu-id="f7ea3-143">Der erteilte Status für die Einwilligung zur Datenfreigabe</span><span class="sxs-lookup"><span data-stu-id="f7ea3-143">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="f7ea3-144">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="f7ea3-144">grantDateTime</span></span>|<span data-ttu-id="f7ea3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7ea3-145">DateTimeOffset</span></span>|<span data-ttu-id="f7ea3-146">Die Zeit Genehmigung für dieses Konto wurde erteilt.</span><span class="sxs-lookup"><span data-stu-id="f7ea3-146">The time consent was granted for this account</span></span>|
|<span data-ttu-id="f7ea3-147">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="f7ea3-147">grantedByUpn</span></span>|<span data-ttu-id="f7ea3-148">String</span><span class="sxs-lookup"><span data-stu-id="f7ea3-148">String</span></span>|<span data-ttu-id="f7ea3-149">Der UPN des Benutzers, der die Einwilligung für dieses Konto erteilt hat.</span><span class="sxs-lookup"><span data-stu-id="f7ea3-149">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="f7ea3-150">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="f7ea3-150">grantedByUserId</span></span>|<span data-ttu-id="f7ea3-151">String</span><span class="sxs-lookup"><span data-stu-id="f7ea3-151">String</span></span>|<span data-ttu-id="f7ea3-152">Die UserId des Benutzers, der die Einwilligung für dieses Konto erteilt hat</span><span class="sxs-lookup"><span data-stu-id="f7ea3-152">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="f7ea3-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7ea3-153">Response</span></span>
<span data-ttu-id="f7ea3-154">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f7ea3-154">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7ea3-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7ea3-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7ea3-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7ea3-156">Request</span></span>
<span data-ttu-id="f7ea3-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f7ea3-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7ea3-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7ea3-158">Response</span></span>
<span data-ttu-id="f7ea3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7ea3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




