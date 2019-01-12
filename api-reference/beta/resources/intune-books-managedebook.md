---
title: managedEBook-Ressourcentyp
description: Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6fd4fd3caef3aab90257805a48e53bee9c6b8764
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962597"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="8d5fd-103">managedEBook-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8d5fd-103">managedEBook resource type</span></span>

> <span data-ttu-id="8d5fd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8d5fd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d5fd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d5fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d5fd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8d5fd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d5fd-107">Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält</span><span class="sxs-lookup"><span data-stu-id="8d5fd-107">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="8d5fd-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="8d5fd-108">Methods</span></span>
|<span data-ttu-id="8d5fd-109">Methode</span><span class="sxs-lookup"><span data-stu-id="8d5fd-109">Method</span></span>|<span data-ttu-id="8d5fd-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8d5fd-110">Return Type</span></span>|<span data-ttu-id="8d5fd-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d5fd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8d5fd-112">managedEBooks auflisten</span><span class="sxs-lookup"><span data-stu-id="8d5fd-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="8d5fd-113">[managedEBook](../resources/intune-books-managedebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8d5fd-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="8d5fd-114">Auflisten von Eigenschaften und Beziehungen der [managedEBook](../resources/intune-books-managedebook.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="8d5fd-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="8d5fd-115">managedEBook abrufen</span><span class="sxs-lookup"><span data-stu-id="8d5fd-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="8d5fd-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="8d5fd-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="8d5fd-117">Lesen von Eigenschaften und Beziehungen des [managedEBook](../resources/intune-books-managedebook.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8d5fd-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="8d5fd-118">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="8d5fd-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="8d5fd-119">Keine</span><span class="sxs-lookup"><span data-stu-id="8d5fd-119">None</span></span>|<span data-ttu-id="8d5fd-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8d5fd-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8d5fd-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8d5fd-121">Properties</span></span>
|<span data-ttu-id="8d5fd-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8d5fd-122">Property</span></span>|<span data-ttu-id="8d5fd-123">Typ</span><span class="sxs-lookup"><span data-stu-id="8d5fd-123">Type</span></span>|<span data-ttu-id="8d5fd-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d5fd-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d5fd-125">id</span><span class="sxs-lookup"><span data-stu-id="8d5fd-125">id</span></span>|<span data-ttu-id="8d5fd-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5fd-126">String</span></span>|<span data-ttu-id="8d5fd-127">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8d5fd-127">Key of the entity.</span></span>|
|<span data-ttu-id="8d5fd-128">displayName</span><span class="sxs-lookup"><span data-stu-id="8d5fd-128">displayName</span></span>|<span data-ttu-id="8d5fd-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5fd-129">String</span></span>|<span data-ttu-id="8d5fd-130">Name des E-Books</span><span class="sxs-lookup"><span data-stu-id="8d5fd-130">Name of the eBook.</span></span>|
|<span data-ttu-id="8d5fd-131">description</span><span class="sxs-lookup"><span data-stu-id="8d5fd-131">description</span></span>|<span data-ttu-id="8d5fd-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5fd-132">String</span></span>|<span data-ttu-id="8d5fd-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d5fd-133">Description.</span></span>|
|<span data-ttu-id="8d5fd-134">publisher</span><span class="sxs-lookup"><span data-stu-id="8d5fd-134">publisher</span></span>|<span data-ttu-id="8d5fd-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5fd-135">String</span></span>|<span data-ttu-id="8d5fd-136">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="8d5fd-136">Publisher.</span></span>|
|<span data-ttu-id="8d5fd-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d5fd-137">publishedDateTime</span></span>|<span data-ttu-id="8d5fd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d5fd-138">DateTimeOffset</span></span>|<span data-ttu-id="8d5fd-139">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="8d5fd-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="8d5fd-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="8d5fd-140">largeCover</span></span>|[<span data-ttu-id="8d5fd-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8d5fd-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8d5fd-142">Umschlagbild des Buchs</span><span class="sxs-lookup"><span data-stu-id="8d5fd-142">Book cover.</span></span>|
|<span data-ttu-id="8d5fd-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d5fd-143">createdDateTime</span></span>|<span data-ttu-id="8d5fd-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d5fd-144">DateTimeOffset</span></span>|<span data-ttu-id="8d5fd-145">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="8d5fd-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="8d5fd-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d5fd-146">lastModifiedDateTime</span></span>|<span data-ttu-id="8d5fd-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d5fd-147">DateTimeOffset</span></span>|<span data-ttu-id="8d5fd-148">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="8d5fd-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="8d5fd-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8d5fd-149">informationUrl</span></span>|<span data-ttu-id="8d5fd-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5fd-150">String</span></span>|<span data-ttu-id="8d5fd-151">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="8d5fd-151">The more information Url.</span></span>|
|<span data-ttu-id="8d5fd-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8d5fd-152">privacyInformationUrl</span></span>|<span data-ttu-id="8d5fd-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d5fd-153">String</span></span>|<span data-ttu-id="8d5fd-154">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="8d5fd-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d5fd-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8d5fd-155">Relationships</span></span>
|<span data-ttu-id="8d5fd-156">Beziehung</span><span class="sxs-lookup"><span data-stu-id="8d5fd-156">Relationship</span></span>|<span data-ttu-id="8d5fd-157">Typ</span><span class="sxs-lookup"><span data-stu-id="8d5fd-157">Type</span></span>|<span data-ttu-id="8d5fd-158">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d5fd-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d5fd-159">categories</span><span class="sxs-lookup"><span data-stu-id="8d5fd-159">categories</span></span>|<span data-ttu-id="8d5fd-160">[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="8d5fd-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="8d5fd-161">Die Liste der Kategorien für e-Book.</span><span class="sxs-lookup"><span data-stu-id="8d5fd-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="8d5fd-162">assignments</span><span class="sxs-lookup"><span data-stu-id="8d5fd-162">assignments</span></span>|<span data-ttu-id="8d5fd-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8d5fd-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="8d5fd-164">Die Liste der Zuweisungen für dieses E-Book.</span><span class="sxs-lookup"><span data-stu-id="8d5fd-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="8d5fd-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="8d5fd-165">installSummary</span></span>|[<span data-ttu-id="8d5fd-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="8d5fd-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="8d5fd-167">Die Installationszusammenfassung für die mobile App.</span><span class="sxs-lookup"><span data-stu-id="8d5fd-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="8d5fd-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="8d5fd-168">deviceStates</span></span>|<span data-ttu-id="8d5fd-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8d5fd-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="8d5fd-170">Die Liste der Installationsstatus für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="8d5fd-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="8d5fd-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="8d5fd-171">userStateSummary</span></span>|<span data-ttu-id="8d5fd-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8d5fd-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="8d5fd-173">Die Liste der Installationsstatus für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="8d5fd-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d5fd-174">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8d5fd-174">JSON Representation</span></span>
<span data-ttu-id="8d5fd-175">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8d5fd-175">Here is a JSON representation of the resource.</span></span>
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





