---
title: managedEBook-Ressourcentyp
description: Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält
author: tfitzmac
ms.openlocfilehash: 7b826d7b0a11ce957a87154f276abc0e8168f45d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347145"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="8f9db-103">managedEBook-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8f9db-103">managedEBook resource type</span></span>

> <span data-ttu-id="8f9db-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8f9db-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f9db-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8f9db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f9db-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8f9db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f9db-107">Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält</span><span class="sxs-lookup"><span data-stu-id="8f9db-107">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="8f9db-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="8f9db-108">Methods</span></span>
|<span data-ttu-id="8f9db-109">Methode</span><span class="sxs-lookup"><span data-stu-id="8f9db-109">Method</span></span>|<span data-ttu-id="8f9db-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8f9db-110">Return Type</span></span>|<span data-ttu-id="8f9db-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f9db-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8f9db-112">managedEBooks auflisten</span><span class="sxs-lookup"><span data-stu-id="8f9db-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="8f9db-113">[managedEBook](../resources/intune-books-managedebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8f9db-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="8f9db-114">Auflisten von Eigenschaften und Beziehungen der [managedEBook](../resources/intune-books-managedebook.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="8f9db-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="8f9db-115">managedEBook abrufen</span><span class="sxs-lookup"><span data-stu-id="8f9db-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="8f9db-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="8f9db-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="8f9db-117">Lesen von Eigenschaften und Beziehungen des [managedEBook](../resources/intune-books-managedebook.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8f9db-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="8f9db-118">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="8f9db-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="8f9db-119">Keine</span><span class="sxs-lookup"><span data-stu-id="8f9db-119">None</span></span>|<span data-ttu-id="8f9db-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8f9db-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8f9db-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8f9db-121">Properties</span></span>
|<span data-ttu-id="8f9db-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f9db-122">Property</span></span>|<span data-ttu-id="8f9db-123">Typ</span><span class="sxs-lookup"><span data-stu-id="8f9db-123">Type</span></span>|<span data-ttu-id="8f9db-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f9db-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f9db-125">id</span><span class="sxs-lookup"><span data-stu-id="8f9db-125">id</span></span>|<span data-ttu-id="8f9db-126">String</span><span class="sxs-lookup"><span data-stu-id="8f9db-126">String</span></span>|<span data-ttu-id="8f9db-127">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8f9db-127">Key of the entity.</span></span>|
|<span data-ttu-id="8f9db-128">displayName</span><span class="sxs-lookup"><span data-stu-id="8f9db-128">displayName</span></span>|<span data-ttu-id="8f9db-129">String</span><span class="sxs-lookup"><span data-stu-id="8f9db-129">String</span></span>|<span data-ttu-id="8f9db-130">Name des E-Books</span><span class="sxs-lookup"><span data-stu-id="8f9db-130">Name of the eBook.</span></span>|
|<span data-ttu-id="8f9db-131">description</span><span class="sxs-lookup"><span data-stu-id="8f9db-131">description</span></span>|<span data-ttu-id="8f9db-132">String</span><span class="sxs-lookup"><span data-stu-id="8f9db-132">String</span></span>|<span data-ttu-id="8f9db-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f9db-133">Description.</span></span>|
|<span data-ttu-id="8f9db-134">publisher</span><span class="sxs-lookup"><span data-stu-id="8f9db-134">publisher</span></span>|<span data-ttu-id="8f9db-135">String</span><span class="sxs-lookup"><span data-stu-id="8f9db-135">String</span></span>|<span data-ttu-id="8f9db-136">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="8f9db-136">Publisher.</span></span>|
|<span data-ttu-id="8f9db-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f9db-137">publishedDateTime</span></span>|<span data-ttu-id="8f9db-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f9db-138">DateTimeOffset</span></span>|<span data-ttu-id="8f9db-139">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="8f9db-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="8f9db-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="8f9db-140">largeCover</span></span>|[<span data-ttu-id="8f9db-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8f9db-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8f9db-142">Umschlagbild des Buchs</span><span class="sxs-lookup"><span data-stu-id="8f9db-142">Book cover.</span></span>|
|<span data-ttu-id="8f9db-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f9db-143">createdDateTime</span></span>|<span data-ttu-id="8f9db-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f9db-144">DateTimeOffset</span></span>|<span data-ttu-id="8f9db-145">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="8f9db-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="8f9db-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f9db-146">lastModifiedDateTime</span></span>|<span data-ttu-id="8f9db-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f9db-147">DateTimeOffset</span></span>|<span data-ttu-id="8f9db-148">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="8f9db-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="8f9db-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8f9db-149">informationUrl</span></span>|<span data-ttu-id="8f9db-150">String</span><span class="sxs-lookup"><span data-stu-id="8f9db-150">String</span></span>|<span data-ttu-id="8f9db-151">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="8f9db-151">The more information Url.</span></span>|
|<span data-ttu-id="8f9db-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8f9db-152">privacyInformationUrl</span></span>|<span data-ttu-id="8f9db-153">String</span><span class="sxs-lookup"><span data-stu-id="8f9db-153">String</span></span>|<span data-ttu-id="8f9db-154">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="8f9db-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f9db-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8f9db-155">Relationships</span></span>
|<span data-ttu-id="8f9db-156">Beziehung</span><span class="sxs-lookup"><span data-stu-id="8f9db-156">Relationship</span></span>|<span data-ttu-id="8f9db-157">Typ</span><span class="sxs-lookup"><span data-stu-id="8f9db-157">Type</span></span>|<span data-ttu-id="8f9db-158">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f9db-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f9db-159">categories</span><span class="sxs-lookup"><span data-stu-id="8f9db-159">categories</span></span>|<span data-ttu-id="8f9db-160">[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="8f9db-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="8f9db-161">Die Liste der Kategorien für e-Book.</span><span class="sxs-lookup"><span data-stu-id="8f9db-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="8f9db-162">assignments</span><span class="sxs-lookup"><span data-stu-id="8f9db-162">assignments</span></span>|<span data-ttu-id="8f9db-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8f9db-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="8f9db-164">Die Liste der Zuweisungen für dieses E-Book.</span><span class="sxs-lookup"><span data-stu-id="8f9db-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="8f9db-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="8f9db-165">installSummary</span></span>|[<span data-ttu-id="8f9db-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="8f9db-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="8f9db-167">Die Installationszusammenfassung für die mobile App.</span><span class="sxs-lookup"><span data-stu-id="8f9db-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="8f9db-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="8f9db-168">deviceStates</span></span>|<span data-ttu-id="8f9db-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8f9db-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="8f9db-170">Die Liste der Installationsstatus für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="8f9db-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="8f9db-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="8f9db-171">userStateSummary</span></span>|<span data-ttu-id="8f9db-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8f9db-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="8f9db-173">Die Liste der Installationsstatus für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="8f9db-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f9db-174">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8f9db-174">JSON Representation</span></span>
<span data-ttu-id="8f9db-175">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8f9db-175">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```





