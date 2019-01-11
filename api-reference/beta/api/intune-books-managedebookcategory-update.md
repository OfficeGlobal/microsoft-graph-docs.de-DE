---
title: ManagedEBookCategory aktualisieren
description: Aktualisieren Sie die Eigenschaften eines ManagedEBookCategory-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ef8970fb32b94b17b9277c3d30fc72bbc582ea87
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853193"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="85e03-103">ManagedEBookCategory aktualisieren</span><span class="sxs-lookup"><span data-stu-id="85e03-103">Update managedEBookCategory</span></span>

> <span data-ttu-id="85e03-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="85e03-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85e03-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85e03-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85e03-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="85e03-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85e03-107">Aktualisieren Sie die Eigenschaften eines [ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="85e03-107">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85e03-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="85e03-108">Prerequisites</span></span>
<span data-ttu-id="85e03-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85e03-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85e03-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="85e03-111">Permission type</span></span>|<span data-ttu-id="85e03-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="85e03-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85e03-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="85e03-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85e03-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85e03-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="85e03-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="85e03-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85e03-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85e03-116">Not supported.</span></span>|
|<span data-ttu-id="85e03-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="85e03-117">Application</span></span>|<span data-ttu-id="85e03-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85e03-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85e03-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="85e03-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="85e03-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="85e03-120">Request headers</span></span>
|<span data-ttu-id="85e03-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="85e03-121">Header</span></span>|<span data-ttu-id="85e03-122">Wert</span><span class="sxs-lookup"><span data-stu-id="85e03-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85e03-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85e03-123">Authorization</span></span>|<span data-ttu-id="85e03-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="85e03-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85e03-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="85e03-125">Accept</span></span>|<span data-ttu-id="85e03-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85e03-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85e03-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="85e03-127">Request body</span></span>
<span data-ttu-id="85e03-128">Geben Sie im Textkörper Anforderung für das Objekt [ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="85e03-128">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="85e03-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [ManagedEBookCategory](../resources/intune-books-managedebookcategory.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="85e03-129">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="85e03-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="85e03-130">Property</span></span>|<span data-ttu-id="85e03-131">Typ</span><span class="sxs-lookup"><span data-stu-id="85e03-131">Type</span></span>|<span data-ttu-id="85e03-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85e03-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85e03-133">id</span><span class="sxs-lookup"><span data-stu-id="85e03-133">id</span></span>|<span data-ttu-id="85e03-134">String</span><span class="sxs-lookup"><span data-stu-id="85e03-134">String</span></span>|<span data-ttu-id="85e03-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="85e03-135">The key of the entity.</span></span>|
|<span data-ttu-id="85e03-136">displayName</span><span class="sxs-lookup"><span data-stu-id="85e03-136">displayName</span></span>|<span data-ttu-id="85e03-137">String</span><span class="sxs-lookup"><span data-stu-id="85e03-137">String</span></span>|<span data-ttu-id="85e03-138">Der Name der Kategorie eBook.</span><span class="sxs-lookup"><span data-stu-id="85e03-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="85e03-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85e03-139">lastModifiedDateTime</span></span>|<span data-ttu-id="85e03-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85e03-140">DateTimeOffset</span></span>|<span data-ttu-id="85e03-141">Datum und Uhrzeit der letzten Änderung der ManagedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="85e03-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="85e03-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="85e03-142">Response</span></span>
<span data-ttu-id="85e03-143">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="85e03-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85e03-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="85e03-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="85e03-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="85e03-145">Request</span></span>
<span data-ttu-id="85e03-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="85e03-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 107

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="85e03-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="85e03-147">Response</span></span>
<span data-ttu-id="85e03-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85e03-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





