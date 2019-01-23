---
title: DataSharingConsent aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DataSharingConsent-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 143e2c655adac2403f49bb92afff2aca30a3653f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421116"
---
# <a name="update-datasharingconsent"></a><span data-ttu-id="e7a89-103">DataSharingConsent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e7a89-103">Update dataSharingConsent</span></span>

> <span data-ttu-id="e7a89-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e7a89-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e7a89-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e7a89-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7a89-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e7a89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7a89-107">Aktualisieren Sie die Eigenschaften eines [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e7a89-107">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7a89-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e7a89-108">Prerequisites</span></span>
<span data-ttu-id="e7a89-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7a89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e7a89-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e7a89-111">Permission type</span></span>|<span data-ttu-id="e7a89-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e7a89-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7a89-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e7a89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7a89-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7a89-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e7a89-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e7a89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7a89-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7a89-116">Not supported.</span></span>|
|<span data-ttu-id="e7a89-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e7a89-117">Application</span></span>|<span data-ttu-id="e7a89-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7a89-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7a89-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7a89-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="request-headers"></a><span data-ttu-id="e7a89-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e7a89-120">Request headers</span></span>
|<span data-ttu-id="e7a89-121">Header</span><span class="sxs-lookup"><span data-stu-id="e7a89-121">Header</span></span>|<span data-ttu-id="e7a89-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e7a89-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7a89-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e7a89-123">Authorization</span></span>|<span data-ttu-id="e7a89-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e7a89-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7a89-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e7a89-125">Accept</span></span>|<span data-ttu-id="e7a89-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7a89-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7a89-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e7a89-127">Request body</span></span>
<span data-ttu-id="e7a89-128">Geben Sie im Textkörper Anforderung für das Objekt [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="e7a89-128">In the request body, supply a JSON representation for the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

<span data-ttu-id="e7a89-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DataSharingConsent](../resources/intune-devices-datasharingconsent.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="e7a89-129">The following table shows the properties that are required when you create the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>

|<span data-ttu-id="e7a89-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e7a89-130">Property</span></span>|<span data-ttu-id="e7a89-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e7a89-131">Type</span></span>|<span data-ttu-id="e7a89-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e7a89-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7a89-133">id</span><span class="sxs-lookup"><span data-stu-id="e7a89-133">id</span></span>|<span data-ttu-id="e7a89-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7a89-134">String</span></span>|<span data-ttu-id="e7a89-135">Die Daten sharing Zustimmung Id</span><span class="sxs-lookup"><span data-stu-id="e7a89-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="e7a89-136">von Ihnen eingegebene Dienstanzeigename</span><span class="sxs-lookup"><span data-stu-id="e7a89-136">serviceDisplayName</span></span>|<span data-ttu-id="e7a89-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7a89-137">String</span></span>|<span data-ttu-id="e7a89-138">Der Anzeigename der Dienst Workflow</span><span class="sxs-lookup"><span data-stu-id="e7a89-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="e7a89-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="e7a89-139">termsUrl</span></span>|<span data-ttu-id="e7a89-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7a89-140">String</span></span>|<span data-ttu-id="e7a89-141">Die TermsUrl für die Datenfreigabe Zustimmung</span><span class="sxs-lookup"><span data-stu-id="e7a89-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="e7a89-142">erteilt</span><span class="sxs-lookup"><span data-stu-id="e7a89-142">granted</span></span>|<span data-ttu-id="e7a89-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7a89-143">Boolean</span></span>|<span data-ttu-id="e7a89-144">Den gewährten Status für die Datenfreigabe Zustimmung</span><span class="sxs-lookup"><span data-stu-id="e7a89-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="e7a89-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="e7a89-145">grantDateTime</span></span>|<span data-ttu-id="e7a89-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7a89-146">DateTimeOffset</span></span>|<span data-ttu-id="e7a89-147">Die Zeit Zustimmung wurde für dieses Konto erteilt.</span><span class="sxs-lookup"><span data-stu-id="e7a89-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="e7a89-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="e7a89-148">grantedByUpn</span></span>|<span data-ttu-id="e7a89-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7a89-149">String</span></span>|<span data-ttu-id="e7a89-150">Den Upn des Benutzers, der für dieses Konto Zustimmung eingeholt</span><span class="sxs-lookup"><span data-stu-id="e7a89-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="e7a89-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="e7a89-151">grantedByUserId</span></span>|<span data-ttu-id="e7a89-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7a89-152">String</span></span>|<span data-ttu-id="e7a89-153">Die Benutzer-ID des Benutzers, der für dieses Konto Zustimmung eingeholt</span><span class="sxs-lookup"><span data-stu-id="e7a89-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="e7a89-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7a89-154">Response</span></span>
<span data-ttu-id="e7a89-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e7a89-155">If successful, this method returns a `200 OK` response code and an updated [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7a89-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e7a89-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7a89-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7a89-157">Request</span></span>
<span data-ttu-id="e7a89-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e7a89-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
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

### <a name="response"></a><span data-ttu-id="e7a89-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7a89-159">Response</span></span>
<span data-ttu-id="e7a89-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e7a89-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




