---
title: EmbeddedSIMActivationCodePool aktualisieren
description: Aktualisieren Sie die Eigenschaften eines EmbeddedSIMActivationCodePool-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1758d832dfbc9fdbc2db1a65259f30c3662b5964
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942934"
---
# <a name="update-embeddedsimactivationcodepool"></a><span data-ttu-id="1968c-103">EmbeddedSIMActivationCodePool aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1968c-103">Update embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="1968c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1968c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1968c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1968c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1968c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1968c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1968c-107">Aktualisieren Sie die Eigenschaften eines [EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1968c-107">Update the properties of a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1968c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1968c-108">Prerequisites</span></span>
<span data-ttu-id="1968c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1968c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1968c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1968c-111">Permission type</span></span>|<span data-ttu-id="1968c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1968c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1968c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1968c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1968c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1968c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1968c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1968c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1968c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1968c-116">Not supported.</span></span>|
|<span data-ttu-id="1968c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1968c-117">Application</span></span>|<span data-ttu-id="1968c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1968c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1968c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1968c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a><span data-ttu-id="1968c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1968c-120">Request headers</span></span>
|<span data-ttu-id="1968c-121">Header</span><span class="sxs-lookup"><span data-stu-id="1968c-121">Header</span></span>|<span data-ttu-id="1968c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1968c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1968c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1968c-123">Authorization</span></span>|<span data-ttu-id="1968c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1968c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1968c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1968c-125">Accept</span></span>|<span data-ttu-id="1968c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1968c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1968c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1968c-127">Request body</span></span>
<span data-ttu-id="1968c-128">Geben Sie im Textkörper Anforderung für das Objekt [EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="1968c-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

<span data-ttu-id="1968c-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="1968c-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>

|<span data-ttu-id="1968c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1968c-130">Property</span></span>|<span data-ttu-id="1968c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1968c-131">Type</span></span>|<span data-ttu-id="1968c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1968c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1968c-133">id</span><span class="sxs-lookup"><span data-stu-id="1968c-133">id</span></span>|<span data-ttu-id="1968c-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1968c-134">String</span></span>|<span data-ttu-id="1968c-135">Eindeutiger Bezeichner für den eingebetteten SIM Aktivierung Code Pool.</span><span class="sxs-lookup"><span data-stu-id="1968c-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="1968c-136">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="1968c-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="1968c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1968c-137">displayName</span></span>|<span data-ttu-id="1968c-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1968c-138">String</span></span>|<span data-ttu-id="1968c-139">Der Administrator definierten Namen des eingebetteten SIM Aktivierung Code Pools.</span><span class="sxs-lookup"><span data-stu-id="1968c-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="1968c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1968c-140">createdDateTime</span></span>|<span data-ttu-id="1968c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1968c-141">DateTimeOffset</span></span>|<span data-ttu-id="1968c-142">Der Zeitpunkt, zu der eingebettete SIM Aktivierung Code Pool erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="1968c-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="1968c-143">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="1968c-143">Generated service side.</span></span>|
|<span data-ttu-id="1968c-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1968c-144">modifiedDateTime</span></span>|<span data-ttu-id="1968c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1968c-145">DateTimeOffset</span></span>|<span data-ttu-id="1968c-146">Der Zeitpunkt der letzten Änderung der eingebettete SIM Aktivierung Code Pool.</span><span class="sxs-lookup"><span data-stu-id="1968c-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="1968c-147">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="1968c-147">Updated service side.</span></span>|
|<span data-ttu-id="1968c-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="1968c-148">activationCodes</span></span>|<span data-ttu-id="1968c-149">[EmbeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="1968c-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="1968c-150">Die Aktivierungscodes in diesem Pool angehören.</span><span class="sxs-lookup"><span data-stu-id="1968c-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="1968c-151">Diese Navigationseigenschaft wird verwendet, um die Aktivierungscodes Intune buchen aber kann nicht zum Lesen von Aktivierungscodes aus Intune verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="1968c-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="1968c-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="1968c-152">activationCodeCount</span></span>|<span data-ttu-id="1968c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="1968c-153">Int32</span></span>|<span data-ttu-id="1968c-154">Die Gesamtzahl der Aktivierungscodes in diesem Pool angehören.</span><span class="sxs-lookup"><span data-stu-id="1968c-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="1968c-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="1968c-155">Response</span></span>
<span data-ttu-id="1968c-156">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1968c-156">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1968c-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1968c-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="1968c-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1968c-158">Request</span></span>
<span data-ttu-id="1968c-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1968c-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
Content-type: application/json
Content-length: 392

{
  "displayName": "Display Name value",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```

### <a name="response"></a><span data-ttu-id="1968c-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="1968c-160">Response</span></span>
<span data-ttu-id="1968c-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1968c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 628

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "ec308741-8741-ec30-4187-30ec418730ec",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```





