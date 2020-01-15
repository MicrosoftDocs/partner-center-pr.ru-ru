---
title: Центр партнеров Insights — управление доступом на основе ролей | Центр партнеров
ms.topic: article
ms.date: 01/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Для просмотра отчетов Insights требуются определенные роли.
ms.assetid: 2F4B9A27-37FF-41E4-8A26-5EAE88DD8A49
keywords: PCI, производительность, успешный клиент, измерения, роли
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e51e86ed20af16d4bc4c5d48b33eee712480bfab
ms.sourcegitcommit: 1a735003cca0bd430195ac1213bd8d77bd5063a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2020
ms.locfileid: "75945866"
---
# <a name="roles-based-access-control-to-the-insights-dashboard"></a><span data-ttu-id="b8911-104">Управление доступом на основе ролей на панели мониторинга Insights</span><span class="sxs-lookup"><span data-stu-id="b8911-104">Roles-based access control to the Insights dashboard</span></span>

<span data-ttu-id="b8911-105">Панель мониторинга Insights использует две новые роли в центре партнеров для управления доступом сотрудников к диспетчеру отчетов и средству просмотра отчетов.</span><span class="sxs-lookup"><span data-stu-id="b8911-105">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="b8911-106">Пользователи в роли средства просмотра отчетов руководителя имеют доступ ко всем наборам данных отчетов, а пользователи в роли средства просмотра отчетов не будут иметь доступ к конфиденциальным наборам, таким как доход, а также персональные данные клиентов и сотрудников.</span><span class="sxs-lookup"><span data-stu-id="b8911-106">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="b8911-107">Как и в случае с другими ролями центра партнеров, глобальный администратор или администратор учетной записи сможет назначить пользователей этим ролям на странице Управление пользователями.</span><span class="sxs-lookup"><span data-stu-id="b8911-107">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="b8911-108">Роли могут быть применимы ко всей компании или к конкретным MPN расположениям.</span><span class="sxs-lookup"><span data-stu-id="b8911-108">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="b8911-109">Роли, назначенные для конкретных расположений MPN, ограничивают пользователя для просмотра данных отчетов, связанных только с выбранными расположениями MPN.</span><span class="sxs-lookup"><span data-stu-id="b8911-109">Roles assigned for specific MPN location(s) limits the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="b8911-110">Партнер может выбрать одно или несколько расположений из приведенного ниже представления.</span><span class="sxs-lookup"><span data-stu-id="b8911-110">Partner can select one or multiple locations from the below view.</span></span>

![Роли](images/pci/roles.png)

><span data-ttu-id="b8911-112">Метим Пользователи, которые являются MPN администраторами на 20 января, 2020 автоматически добавляются в роль "Executive Report Viewer" всей компании для всех расположений для этого клиента.</span><span class="sxs-lookup"><span data-stu-id="b8911-112">[Note] Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide ‘Executive Report Viewer’ role for all locations for that tenant.</span></span> <span data-ttu-id="b8911-113">Таким образом, эти пользователи могут получить доступ к отчетам в качестве средства просмотра отчетов руководителя без явного действия, необходимого глобальному администратору или администратору учетной записи. Глобальные администраторы и администраторы учетных записей могут переопределять автоматические назначенные роли этих пользователей для дальнейшего увеличения или ограничения их возможностей.</span><span class="sxs-lookup"><span data-stu-id="b8911-113">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>