С помощью команды fdisk -l смотрим какие диски у нас есть
![дз 2 1](https://github.com/DronZap/linux_admin_2/assets/145288949/e3359087-471d-40c9-91be-740896620581)

Зануляем суперблоки выбранных дисков, на случай если диски использовались в других рейдах.

![дз 2 2](https://github.com/DronZap/linux_admin_2/assets/145288949/e5b3637e-af8f-4071-ac70-d8ce434196bf)

Создаем рейд 1, состоящий из двух дисков sdb и sdc.

![дз 2 3](https://github.com/DronZap/linux_admin_2/assets/145288949/736571d6-41dd-4e6d-b804-5f17f9ed0ab2)

Проверяем, что рейд собран нормально.

![дз 2 4](https://github.com/DronZap/linux_admin_2/assets/145288949/4faffc50-fce5-4df0-9a62-713e1bc2546e)
![дз 2 5](https://github.com/DronZap/linux_admin_2/assets/145288949/517eb4b5-6a29-45af-bb4b-0298851cf9ff)

Проверяем информацию о рейде.

![дз 2 6](https://github.com/DronZap/linux_admin_2/assets/145288949/aee1a347-498e-4f69-881f-3c12970039e7)

Создаем файл mdadm.conf

![дз 2 7](https://github.com/DronZap/linux_admin_2/assets/145288949/33fc4402-382b-4ed2-a6d1-5fe97c23bf7c)

Искусственно ломаем диск sdc и проверяем рейд.

![дз 2 8](https://github.com/DronZap/linux_admin_2/assets/145288949/e5bac7f4-e432-462c-a6db-2f6b1b71aace)

Удаляем сломанный диск и добавляем новый диск в рейд. Далее проверяем стадию rebuilding.

![дз 2 9](https://github.com/DronZap/linux_admin_2/assets/145288949/c01e289b-a652-4a9a-bbd3-5be6d7f3a599)

Создаем метку диска gpt на рейде. Далее создаем 5 одинаковых разделов.

![дз 2 10](https://github.com/DronZap/linux_admin_2/assets/145288949/367523a1-9d4d-4c75-8b0a-0e925f999991)

Смотрим созданные разделы на рейде.

![дз 2 11](https://github.com/DronZap/linux_admin_2/assets/145288949/064ff49f-9bb5-4bb9-81bd-447c2ea1e051)

Форматируем разделы на рейде в формате ext4.

![дз 2 12](https://github.com/DronZap/linux_admin_2/assets/145288949/999b44ac-a260-4ad3-9fe4-49c34c07337f)

![дз 2 13](https://github.com/DronZap/linux_admin_2/assets/145288949/c68f1316-ddeb-47fa-9f18-283e5b7e9770)

Монтируем разделы по каталогам

![дз 2 14](https://github.com/DronZap/linux_admin_2/assets/145288949/defee8e2-4326-4fa3-bfea-8bd6f5b69d16)

![дз 2 15](https://github.com/DronZap/linux_admin_2/assets/145288949/da59c150-d705-49af-b7b1-c4f6bf34b9fc)
