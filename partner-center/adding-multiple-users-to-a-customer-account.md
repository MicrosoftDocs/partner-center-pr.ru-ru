---
title: Добавление нескольких пользователей для учетной записи клиента
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Чтобы добавить нескольких пользователей в учетную запись клиента, отправьте файл данных в центр партнеров, используя формат файла значений с разделителями-запятыми (CSV).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150477"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="90a13-103">Передача CSV-файла пользователей в учетную запись клиента</span><span class="sxs-lookup"><span data-stu-id="90a13-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="90a13-104">**Соответствующие роли** — глобальный администратор.</span><span class="sxs-lookup"><span data-stu-id="90a13-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="90a13-105">Одновременное добавление нескольких пользователей в учетную запись клиента путем отправки файла данных в формате файла с разделителями-запятыми (CSV) в центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="90a13-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="90a13-106">Создание файла пользователей клиентов и отправка их в учетную запись клиента</span><span class="sxs-lookup"><span data-stu-id="90a13-106">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="90a13-107">Создайте файл данных с разделителями-запятыми (CSV) с данными, описанными выше.</span><span class="sxs-lookup"><span data-stu-id="90a13-107">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="90a13-108">Сохраните файл, чтобы выбрать его позднее.</span><span class="sxs-lookup"><span data-stu-id="90a13-108">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="90a13-109">[Чтобы импортировать нескольких пользователей для учетной записи клиента, см. поля для CSV-файла](file-customer-users.md).</span><span class="sxs-lookup"><span data-stu-id="90a13-109">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="90a13-110">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="90a13-110">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="90a13-111">В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="90a13-111">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="90a13-112">Выберите вкладку **Пользователи и лицензии** клиента, а затем щелкните **отправить пользователей**.</span><span class="sxs-lookup"><span data-stu-id="90a13-112">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="90a13-113">В разделе **Передача данных пользователя** нажмите кнопку **Обзор**.</span><span class="sxs-lookup"><span data-stu-id="90a13-113">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="90a13-114">В средство выбора файлов выберите ваш файл данных, а затем нажмите **Открыть**.</span><span class="sxs-lookup"><span data-stu-id="90a13-114">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="90a13-115">Выберите **Проверить**.</span><span class="sxs-lookup"><span data-stu-id="90a13-115">Select **Validate**.</span></span>

    <span data-ttu-id="90a13-116">**Примечание**. Большинство ошибок при создании учетной записи вызваны проблемами с файлом данных, такими как отсутствие информации, некорректные или повторяющиеся электронные адреса, слишком много записей в файле и т. д.</span><span class="sxs-lookup"><span data-stu-id="90a13-116">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="90a13-117">После того как центр партнеров проверит файл, выберите географическое **Расположение** для новых пользователей.</span><span class="sxs-lookup"><span data-stu-id="90a13-117">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="90a13-118">Щелкните **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="90a13-118">Select **Save**.</span></span>
10. <span data-ttu-id="90a13-119">Скачайте временный пароль нового пользователя.</span><span class="sxs-lookup"><span data-stu-id="90a13-119">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="90a13-120">Не забудьте скачать файл с временными паролями, так как вы не сможете сделать это позже.</span><span class="sxs-lookup"><span data-stu-id="90a13-120">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="90a13-121">Новым пользователям необходимо выполнить вход в новую учетную запись, используя временный пароль.</span><span class="sxs-lookup"><span data-stu-id="90a13-121">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="90a13-122">Новым пользователям автоматически назначаются разрешения для **использования лицензий и служб**.</span><span class="sxs-lookup"><span data-stu-id="90a13-122">New users are automatically assigned permissions of **Can use licenses and services**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="90a13-123">Следующие шаги</span><span class="sxs-lookup"><span data-stu-id="90a13-123">Next steps</span></span>

- [<span data-ttu-id="90a13-124">Предоставление клиентам доступа в центре партнеров для приобретения своих продуктов или услуг</span><span class="sxs-lookup"><span data-stu-id="90a13-124">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
