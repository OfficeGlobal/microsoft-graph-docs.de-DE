---
title: TermsAndConditionsGroupAssignment aktualisieren
description: Aktualisieren Sie die Eigenschaften eines TermsAndConditionsGroupAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 003713e436e20dbcec9ee6ec1ab6999256fee0b2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891210"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="61a06-103">TermsAndConditionsGroupAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="61a06-103">Update termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="61a06-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="61a06-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61a06-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="61a06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61a06-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="61a06-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61a06-107">Aktualisieren Sie die Eigenschaften eines [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="61a06-107">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="61a06-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="61a06-108">Prerequisites</span></span>
<span data-ttu-id="61a06-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61a06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61a06-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="61a06-111">Permission type</span></span>|<span data-ttu-id="61a06-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="61a06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61a06-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="61a06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61a06-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61a06-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="61a06-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="61a06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61a06-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61a06-116">Not supported.</span></span>|
|<span data-ttu-id="61a06-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="61a06-117">Application</span></span>|<span data-ttu-id="61a06-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61a06-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61a06-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="61a06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="61a06-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="61a06-120">Request headers</span></span>
|<span data-ttu-id="61a06-121">Header</span><span class="sxs-lookup"><span data-stu-id="61a06-121">Header</span></span>|<span data-ttu-id="61a06-122">Wert</span><span class="sxs-lookup"><span data-stu-id="61a06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61a06-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="61a06-123">Authorization</span></span>|<span data-ttu-id="61a06-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="61a06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61a06-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="61a06-125">Accept</span></span>|<span data-ttu-id="61a06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61a06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61a06-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="61a06-127">Request body</span></span>
<span data-ttu-id="61a06-128">Geben Sie im Textkörper Anforderung für das Objekt [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="61a06-128">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="61a06-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="61a06-129">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="61a06-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61a06-130">Property</span></span>|<span data-ttu-id="61a06-131">Typ</span><span class="sxs-lookup"><span data-stu-id="61a06-131">Type</span></span>|<span data-ttu-id="61a06-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61a06-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61a06-133">id</span><span class="sxs-lookup"><span data-stu-id="61a06-133">id</span></span>|<span data-ttu-id="61a06-134">String</span><span class="sxs-lookup"><span data-stu-id="61a06-134">String</span></span>|<span data-ttu-id="61a06-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="61a06-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="61a06-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="61a06-136">targetGroupId</span></span>|<span data-ttu-id="61a06-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="61a06-137">String</span></span>|<span data-ttu-id="61a06-138">Eindeutiger Bezeichner der einer Gruppe, der die Richtlinie T & C zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="61a06-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="61a06-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="61a06-139">Response</span></span>
<span data-ttu-id="61a06-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="61a06-140">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61a06-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="61a06-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="61a06-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="61a06-142">Request</span></span>
<span data-ttu-id="61a06-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61a06-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 48

{
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="61a06-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="61a06-144">Response</span></span>
<span data-ttu-id="61a06-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="61a06-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 169

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
  "targetGroupId": "Target Group Id value"
}
```





