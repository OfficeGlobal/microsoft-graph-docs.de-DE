---
title: Aktualisieren von „termsAndConditionsAcceptanceStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs termsAndConditionsAcceptanceStatus.
ms.openlocfilehash: 4078cc304e85b360b7156235105fc9a0e4949402
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016556"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="c8aa6-103">Aktualisieren von „termsAndConditionsAcceptanceStatus“</span><span class="sxs-lookup"><span data-stu-id="c8aa6-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="c8aa6-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c8aa6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8aa6-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="c8aa6-105">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8aa6-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c8aa6-106">Prerequisites</span></span>
<span data-ttu-id="c8aa6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8aa6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8aa6-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8aa6-109">Permission type</span></span>|<span data-ttu-id="c8aa6-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8aa6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8aa6-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8aa6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c8aa6-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8aa6-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c8aa6-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8aa6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8aa6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8aa6-114">Not supported.</span></span>|
|<span data-ttu-id="c8aa6-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8aa6-115">Application</span></span>|<span data-ttu-id="c8aa6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8aa6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8aa6-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8aa6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="c8aa6-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8aa6-118">Request headers</span></span>
|<span data-ttu-id="c8aa6-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c8aa6-119">Header</span></span>|<span data-ttu-id="c8aa6-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c8aa6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8aa6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8aa6-121">Authorization</span></span>|<span data-ttu-id="c8aa6-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c8aa6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8aa6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c8aa6-123">Accept</span></span>|<span data-ttu-id="c8aa6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c8aa6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8aa6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8aa6-125">Request body</span></span>
<span data-ttu-id="c8aa6-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="c8aa6-126">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="c8aa6-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="c8aa6-127">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="c8aa6-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c8aa6-128">Property</span></span>|<span data-ttu-id="c8aa6-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c8aa6-129">Type</span></span>|<span data-ttu-id="c8aa6-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8aa6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8aa6-131">id</span><span class="sxs-lookup"><span data-stu-id="c8aa6-131">id</span></span>|<span data-ttu-id="c8aa6-132">String</span><span class="sxs-lookup"><span data-stu-id="c8aa6-132">String</span></span>|<span data-ttu-id="c8aa6-133">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="c8aa6-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="c8aa6-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c8aa6-134">userDisplayName</span></span>|<span data-ttu-id="c8aa6-135">String</span><span class="sxs-lookup"><span data-stu-id="c8aa6-135">String</span></span>|<span data-ttu-id="c8aa6-136">Anzeigename des Benutzers, dessen Zustimmung die Entität darstellt</span><span class="sxs-lookup"><span data-stu-id="c8aa6-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="c8aa6-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="c8aa6-137">acceptedVersion</span></span>|<span data-ttu-id="c8aa6-138">Int32</span><span class="sxs-lookup"><span data-stu-id="c8aa6-138">Int32</span></span>|<span data-ttu-id="c8aa6-139">Die Versionsnummer der neuesten Version der Geschäftsbedingungen, die der Benutzer akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="c8aa6-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="c8aa6-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8aa6-140">acceptedDateTime</span></span>|<span data-ttu-id="c8aa6-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8aa6-141">DateTimeOffset</span></span>|<span data-ttu-id="c8aa6-142">Datum und Uhrzeit der letzten Zustimmung zu den Bedingungen durch den Benutzer</span><span class="sxs-lookup"><span data-stu-id="c8aa6-142">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="c8aa6-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8aa6-143">Response</span></span>
<span data-ttu-id="c8aa6-144">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c8aa6-144">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8aa6-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8aa6-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8aa6-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8aa6-146">Request</span></span>
<span data-ttu-id="c8aa6-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8aa6-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="c8aa6-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8aa6-148">Response</span></span>
<span data-ttu-id="c8aa6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8aa6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



