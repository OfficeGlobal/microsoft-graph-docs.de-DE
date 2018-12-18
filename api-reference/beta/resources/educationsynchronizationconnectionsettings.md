---
title: Ressourcentyp educationSynchronizationConnectionSettings
description: 'Stellt die Einstellungen für die Anbieter-Verbindung dar. Dadurch wird das System wissen, wie Sie mit der Anbieter APIs verbinden. '
author: mmast-msft
ms.openlocfilehash: 4e8b62a46fa6d14508a9d57ffedc46411910433d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350624"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="eb0e8-104">Ressourcentyp educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="eb0e8-104">educationSynchronizationConnectionSettings resource type</span></span>

> <span data-ttu-id="eb0e8-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eb0e8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb0e8-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eb0e8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eb0e8-107">Stellt die Einstellungen für die Anbieter-Verbindung dar.</span><span class="sxs-lookup"><span data-stu-id="eb0e8-107">Represents the provider connection settings.</span></span> <span data-ttu-id="eb0e8-108">Dadurch wird das System wissen, wie Sie mit der Anbieter APIs verbinden.</span><span class="sxs-lookup"><span data-stu-id="eb0e8-108">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="eb0e8-109">**Hinweis:** Dieser komplexe Typ ist abstrakt.</span><span class="sxs-lookup"><span data-stu-id="eb0e8-109">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="eb0e8-110">Verweisen Sie auf die bestimmten Arten von Verbindungseinstellungen aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="eb0e8-110">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="eb0e8-111">Abgeleitete Typen</span><span class="sxs-lookup"><span data-stu-id="eb0e8-111">Derived types</span></span>
| <span data-ttu-id="eb0e8-112">Typ</span><span class="sxs-lookup"><span data-stu-id="eb0e8-112">Type</span></span> | <span data-ttu-id="eb0e8-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb0e8-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="eb0e8-114">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="eb0e8-114">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="eb0e8-115">Verwenden Sie diesen Typ OAuth1 Verbindungseinstellungen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="eb0e8-115">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="eb0e8-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="eb0e8-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="eb0e8-117">Verwenden Sie diesen Typ OAuth2 Client Anmeldeinformationen Grant-Verbindungseinstellungen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="eb0e8-117">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="eb0e8-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eb0e8-118">Properties</span></span>

| <span data-ttu-id="eb0e8-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eb0e8-119">Property</span></span> | <span data-ttu-id="eb0e8-120">Typ</span><span class="sxs-lookup"><span data-stu-id="eb0e8-120">Type</span></span> | <span data-ttu-id="eb0e8-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb0e8-121">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="eb0e8-122">**clientId**</span><span class="sxs-lookup"><span data-stu-id="eb0e8-122">**clientId**</span></span> | <span data-ttu-id="eb0e8-123">String</span><span class="sxs-lookup"><span data-stu-id="eb0e8-123">String</span></span> |  <span data-ttu-id="eb0e8-124">Client-ID für die Verbindung an den Anbieter verwendet.</span><span class="sxs-lookup"><span data-stu-id="eb0e8-124">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="eb0e8-125">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="eb0e8-125">**clientSecret**</span></span> | <span data-ttu-id="eb0e8-126">String</span><span class="sxs-lookup"><span data-stu-id="eb0e8-126">String</span></span> |  <span data-ttu-id="eb0e8-127">Geheimer Clientschlüssel zum Authentifizieren der Verbindungs an den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="eb0e8-127">Client secret to authenticate the connection to the provider.</span></span> |