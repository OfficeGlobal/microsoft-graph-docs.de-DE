---
title: DataSharingConsent aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DataSharingConsent-Objekts.
author: tfitzmac
ms.openlocfilehash: 1d7759def9c11165fca0b646f166ac792c14369e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317633"
---
# <a name="update-datasharingconsent"></a><span data-ttu-id="36e42-103">DataSharingConsent aktualisieren</span><span class="sxs-lookup"><span data-stu-id="36e42-103">Update dataSharingConsent</span></span>

> <span data-ttu-id="36e42-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="36e42-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36e42-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="36e42-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36e42-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="36e42-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36e42-107">Aktualisieren Sie die Eigenschaften eines [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="36e42-107">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36e42-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="36e42-108">Prerequisites</span></span>
<span data-ttu-id="36e42-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36e42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36e42-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="36e42-111">Permission type</span></span>|<span data-ttu-id="36e42-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="36e42-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36e42-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="36e42-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36e42-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36e42-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="36e42-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="36e42-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36e42-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36e42-116">Not supported.</span></span>|
|<span data-ttu-id="36e42-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="36e42-117">Application</span></span>|<span data-ttu-id="36e42-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36e42-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36e42-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="36e42-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="request-headers"></a><span data-ttu-id="36e42-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="36e42-120">Request headers</span></span>
|<span data-ttu-id="36e42-121">Header</span><span class="sxs-lookup"><span data-stu-id="36e42-121">Header</span></span>|<span data-ttu-id="36e42-122">Wert</span><span class="sxs-lookup"><span data-stu-id="36e42-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36e42-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="36e42-123">Authorization</span></span>|<span data-ttu-id="36e42-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="36e42-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36e42-125">Accept</span><span class="sxs-lookup"><span data-stu-id="36e42-125">Accept</span></span>|<span data-ttu-id="36e42-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36e42-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36e42-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="36e42-127">Request body</span></span>
<span data-ttu-id="36e42-128">Geben Sie im Textkörper Anforderung für das Objekt [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="36e42-128">In the request body, supply a JSON representation for the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

<span data-ttu-id="36e42-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DataSharingConsent](../resources/intune-devices-datasharingconsent.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="36e42-129">The following table shows the properties that are required when you create the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>

|<span data-ttu-id="36e42-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="36e42-130">Property</span></span>|<span data-ttu-id="36e42-131">Typ</span><span class="sxs-lookup"><span data-stu-id="36e42-131">Type</span></span>|<span data-ttu-id="36e42-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36e42-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36e42-133">id</span><span class="sxs-lookup"><span data-stu-id="36e42-133">id</span></span>|<span data-ttu-id="36e42-134">String</span><span class="sxs-lookup"><span data-stu-id="36e42-134">String</span></span>|<span data-ttu-id="36e42-135">Die Daten sharing Zustimmung Id</span><span class="sxs-lookup"><span data-stu-id="36e42-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="36e42-136">von Ihnen eingegebene Dienstanzeigename</span><span class="sxs-lookup"><span data-stu-id="36e42-136">serviceDisplayName</span></span>|<span data-ttu-id="36e42-137">String</span><span class="sxs-lookup"><span data-stu-id="36e42-137">String</span></span>|<span data-ttu-id="36e42-138">Der Anzeigename der Dienst Workflow</span><span class="sxs-lookup"><span data-stu-id="36e42-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="36e42-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="36e42-139">termsUrl</span></span>|<span data-ttu-id="36e42-140">String</span><span class="sxs-lookup"><span data-stu-id="36e42-140">String</span></span>|<span data-ttu-id="36e42-141">Die TermsUrl für die Datenfreigabe Zustimmung</span><span class="sxs-lookup"><span data-stu-id="36e42-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="36e42-142">erteilt</span><span class="sxs-lookup"><span data-stu-id="36e42-142">granted</span></span>|<span data-ttu-id="36e42-143">Boolesch</span><span class="sxs-lookup"><span data-stu-id="36e42-143">Boolean</span></span>|<span data-ttu-id="36e42-144">Den gewährten Status für die Datenfreigabe Zustimmung</span><span class="sxs-lookup"><span data-stu-id="36e42-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="36e42-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="36e42-145">grantDateTime</span></span>|<span data-ttu-id="36e42-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36e42-146">DateTimeOffset</span></span>|<span data-ttu-id="36e42-147">Die Zeit Zustimmung wurde für dieses Konto erteilt.</span><span class="sxs-lookup"><span data-stu-id="36e42-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="36e42-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="36e42-148">grantedByUpn</span></span>|<span data-ttu-id="36e42-149">String</span><span class="sxs-lookup"><span data-stu-id="36e42-149">String</span></span>|<span data-ttu-id="36e42-150">Den Upn des Benutzers, der für dieses Konto Zustimmung eingeholt</span><span class="sxs-lookup"><span data-stu-id="36e42-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="36e42-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="36e42-151">grantedByUserId</span></span>|<span data-ttu-id="36e42-152">String</span><span class="sxs-lookup"><span data-stu-id="36e42-152">String</span></span>|<span data-ttu-id="36e42-153">Die Benutzer-ID des Benutzers, der für dieses Konto Zustimmung eingeholt</span><span class="sxs-lookup"><span data-stu-id="36e42-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="36e42-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="36e42-154">Response</span></span>
<span data-ttu-id="36e42-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="36e42-155">If successful, this method returns a `200 OK` response code and an updated [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36e42-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="36e42-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="36e42-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="36e42-157">Request</span></span>
<span data-ttu-id="36e42-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="36e42-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
Content-type: application/json
Content-length: 276

{
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```

### <a name="response"></a><span data-ttu-id="36e42-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="36e42-159">Response</span></span>
<span data-ttu-id="36e42-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36e42-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





