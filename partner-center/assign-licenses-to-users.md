---
title: Управление пользователями в клиентских учетных записях
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как создавать учетные записи пользователей для клиентов, добавлять или удалять пользовательские лицензии, сбрасывать пароли пользователей, удалять учетные записи пользователей и восстанавливать их.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a3febadda51094d443d83d17b640b1744a130335
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527680"
---
# <a name="user-management-tasks-for-customer-accounts-in-partner-center"></a><span data-ttu-id="2d0fa-103">Задачи управления пользователями для учетных записей клиентов в центре партнеров</span><span class="sxs-lookup"><span data-stu-id="2d0fa-103">User management tasks for customer accounts in Partner Center</span></span>

<span data-ttu-id="2d0fa-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="2d0fa-104">**Applies to**</span></span>

- <span data-ttu-id="2d0fa-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="2d0fa-105">Partner Center</span></span>

<span data-ttu-id="2d0fa-106">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="2d0fa-106">**Appropriate roles**</span></span>

- <span data-ttu-id="2d0fa-107">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="2d0fa-107">Global admin</span></span>
- <span data-ttu-id="2d0fa-108">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="2d0fa-108">User management admin</span></span>
- <span data-ttu-id="2d0fa-109">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="2d0fa-109">Admin agent</span></span>
- <span data-ttu-id="2d0fa-110">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="2d0fa-110">Sales agent</span></span>
- <span data-ttu-id="2d0fa-111">Агент службы технической поддержки</span><span class="sxs-lookup"><span data-stu-id="2d0fa-111">Helpdesk agent</span></span>

<span data-ttu-id="2d0fa-112">Вы можете создавать и удалять новых пользователей в учетной записи клиента.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-112">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="2d0fa-113">Вы также можете восстановить одну или несколько учетных записей пользователей, которые ранее были удалены в течение 30 дней после удаления.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-113">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="2d0fa-114">Предыдущие подписки пользователя также будут восстановлены (если они доступны).</span><span class="sxs-lookup"><span data-stu-id="2d0fa-114">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="2d0fa-115">При покупке новых подписок для клиента Клиент должен предоставить вам список всех пользователей, которым понадобятся учетные записи, разрешения пользователей и службы, необходимые для каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-115">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="2d0fa-116">Вы можете [назначить подписки нескольким пользователям](bulk-license-provisioning-for-multiple-users.md) одновременно, импортируя их имена с помощью [CSV-файла Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="2d0fa-116">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="2d0fa-117">Создание учетных записей пользователей для клиента</span><span class="sxs-lookup"><span data-stu-id="2d0fa-117">Create user accounts for a customer</span></span>

1. <span data-ttu-id="2d0fa-118">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-118">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="2d0fa-119">В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-119">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="2d0fa-120">В меню клиента выберите **Users and licenses** (Пользователи и лицензии).</span><span class="sxs-lookup"><span data-stu-id="2d0fa-120">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="2d0fa-121">Для каждого пользователя нажмите кнопку **Добавить пользователя**, а затем внесите сведения, включая данные о разрешениях и лицензиях.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-121">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="2d0fa-122">**Сохраните** внесенные изменения.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-122">**Save** your changes.</span></span>

5. <span data-ttu-id="2d0fa-123">Не забудьте записать имя пользователя и временный пароль, чтобы отправить их пользователю.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-123">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="2d0fa-124">Если вы добавляете несколько пользователей одновременно, выберите пункт **Добавить еще одного пользователя**.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-124">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="2d0fa-125">Вы также можете добавить несколько пользователей одновременно, [импортируя CSV-файл Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="2d0fa-125">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="2d0fa-126">Вы можете дождаться завершения обработки всех пользователей, прежде чем отправить или распечатать имена и пароли на экране подтверждения.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-126">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="2d0fa-127">добавление и удаление пользовательских лицензий для клиента;</span><span class="sxs-lookup"><span data-stu-id="2d0fa-127">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="2d0fa-128">Следующие шаги применяются для добавления или удаления пользовательских лицензий для продуктов Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-128">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="2d0fa-129">Сведения о добавлении или удалении пользовательских лицензий для подписок SaaS на основе лицензий в коммерческом магазине см. в статье [Добавление и удаление лицензий для подписки SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="2d0fa-129">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="2d0fa-130">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-130">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="2d0fa-131">В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-131">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="2d0fa-132">В меню клиента выберите **Users and licenses** (Пользователи и лицензии).</span><span class="sxs-lookup"><span data-stu-id="2d0fa-132">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="2d0fa-133">Выберите одного или несколько пользователей в списке.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-133">Choose one or more users from the list.</span></span> <span data-ttu-id="2d0fa-134">Например, если клиент только что приобрел новые лицензии и вам необходимо назначить их пользователям, у которых их еще нет, можно использовать параметр **Фильтровать пользователей по...**, чтобы найти подходящую группу.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-134">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="2d0fa-135">Выберите элемент **Управление лицензиями**.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-135">Select **Manage licenses**.</span></span> <span data-ttu-id="2d0fa-136">Внесите необходимые изменения и нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-136">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="2d0fa-137">Для [продуктов Azure Marketplace](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)Назначение лицензий и активация управляются с помощью независимого поставщика программного обеспечения, опубликовавшего продукт.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-137">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="2d0fa-138">сброс пароля пользователя для клиента;</span><span class="sxs-lookup"><span data-stu-id="2d0fa-138">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="2d0fa-139">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-139">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="2d0fa-140">В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-140">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="2d0fa-141">В меню клиента выберите **Users and licenses** (Пользователи и лицензии).</span><span class="sxs-lookup"><span data-stu-id="2d0fa-141">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="2d0fa-142">Выберите пользователя из списка.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-142">Choose the user from the list.</span></span>

4.  <span data-ttu-id="2d0fa-143">Внизу экрана нажмите кнопку **Сбросить пароль**.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-143">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="2d0fa-144">Отправьте новый временный пароль пользователю.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-144">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="2d0fa-145">Удаление учетных записей пользователей для клиента</span><span class="sxs-lookup"><span data-stu-id="2d0fa-145">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="2d0fa-146">В меню **Центр партнеров** выберите **Customers (клиенты**).</span><span class="sxs-lookup"><span data-stu-id="2d0fa-146">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="2d0fa-147">Выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-147">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="2d0fa-148">В меню клиента выберите **Users and licenses** (Пользователи и лицензии).</span><span class="sxs-lookup"><span data-stu-id="2d0fa-148">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="2d0fa-149">Выберите пользователя из списка.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-149">Choose the user from the list.</span></span>

3.  <span data-ttu-id="2d0fa-150">В нижней части экрана щелкните **Удалить пользователя**.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-150">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="2d0fa-151">Если потребуется восстановить эту учетную запись, ее можно будет найти на вкладке **Удаленные пользователи** списка **Пользователи и лицензии** клиента.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-151">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="2d0fa-152">Восстановить удаленного пользователя можно в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-152">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="2d0fa-153">восстановление удаленных учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-153">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="2d0fa-154">В меню **Центр партнеров** выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-154">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="2d0fa-155">Выберите **Пользователи и лицензии**.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-155">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="2d0fa-156">Откройте вкладку **Удаленные пользователи ()**. При наличии удаленных пользователей, которых можно восстановить, на ней должно быть показано **(1)** или большее значение.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-156">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="2d0fa-157">Установите один или несколько флажков удаленных пользователей, а затем нажмите кнопку **Восстановить**.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-157">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="2d0fa-158">Все выбранные учетные записи пользователей появятся на странице **Пользователи и лицензии**.</span><span class="sxs-lookup"><span data-stu-id="2d0fa-158">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="2d0fa-159">Связанные темы</span><span class="sxs-lookup"><span data-stu-id="2d0fa-159">Related topics</span></span>


[<span data-ttu-id="2d0fa-160">Назначение и отзыв лицензий для нескольких пользователей</span><span class="sxs-lookup"><span data-stu-id="2d0fa-160">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="2d0fa-161">Создание нескольких пользователей для учетной записи клиента</span><span class="sxs-lookup"><span data-stu-id="2d0fa-161">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)