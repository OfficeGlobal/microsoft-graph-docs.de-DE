---
title: Aktualisieren von „termsAndConditionsAcceptanceStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs termsAndConditionsAcceptanceStatus.
ms.openlocfilehash: 46e7c69be6dc0ac410162b491b51c6f81a65fce5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064716"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="2633a-103">Aktualisieren von „termsAndConditionsAcceptanceStatus“</span><span class="sxs-lookup"><span data-stu-id="2633a-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="2633a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2633a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2633a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2633a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2633a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2633a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2633a-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="2633a-107">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2633a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2633a-108">Prerequisites</span></span>
<span data-ttu-id="2633a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2633a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2633a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2633a-111">Permission type</span></span>|<span data-ttu-id="2633a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2633a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2633a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2633a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2633a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2633a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2633a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2633a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2633a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2633a-116">Not supported.</span></span>|
|<span data-ttu-id="2633a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2633a-117">Application</span></span>|<span data-ttu-id="2633a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2633a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2633a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2633a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="2633a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2633a-120">Request headers</span></span>
|<span data-ttu-id="2633a-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2633a-121">Header</span></span>|<span data-ttu-id="2633a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2633a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2633a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2633a-123">Authorization</span></span>|<span data-ttu-id="2633a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2633a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2633a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2633a-125">Accept</span></span>|<span data-ttu-id="2633a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2633a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2633a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2633a-127">Request body</span></span>
<span data-ttu-id="2633a-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="2633a-128">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="2633a-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2633a-129">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="2633a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2633a-130">Property</span></span>|<span data-ttu-id="2633a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2633a-131">Type</span></span>|<span data-ttu-id="2633a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2633a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2633a-133">id</span><span class="sxs-lookup"><span data-stu-id="2633a-133">id</span></span>|<span data-ttu-id="2633a-134">String</span><span class="sxs-lookup"><span data-stu-id="2633a-134">String</span></span>|<span data-ttu-id="2633a-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="2633a-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="2633a-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2633a-136">userDisplayName</span></span>|<span data-ttu-id="2633a-137">String</span><span class="sxs-lookup"><span data-stu-id="2633a-137">String</span></span>|<span data-ttu-id="2633a-138">Anzeigename des Benutzers, dessen Zustimmung die Entität darstellt</span><span class="sxs-lookup"><span data-stu-id="2633a-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="2633a-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="2633a-139">acceptedVersion</span></span>|<span data-ttu-id="2633a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2633a-140">Int32</span></span>|<span data-ttu-id="2633a-141">Die Versionsnummer der neuesten Version der Geschäftsbedingungen, die der Benutzer akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="2633a-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="2633a-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="2633a-142">acceptedDateTime</span></span>|<span data-ttu-id="2633a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2633a-143">DateTimeOffset</span></span>|<span data-ttu-id="2633a-144">Datum und Uhrzeit der letzten Zustimmung zu den Bedingungen durch den Benutzer</span><span class="sxs-lookup"><span data-stu-id="2633a-144">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="2633a-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="2633a-145">Response</span></span>
<span data-ttu-id="2633a-146">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2633a-146">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2633a-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2633a-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="2633a-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2633a-148">Request</span></span>
<span data-ttu-id="2633a-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2633a-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 138

{
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="2633a-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="2633a-150">Response</span></span>
<span data-ttu-id="2633a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2633a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```





