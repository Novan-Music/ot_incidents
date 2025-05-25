# Label Guide – OT-Cyber Incidents UA/EN v1

| Поле            | Опис                                              | Формат                                        |
|-----------------|---------------------------------------------------|-----------------------------------------------|
| `id`            | Унікальний ідентифікатор інциденту                | `string` (UUID, CVE або власний ключ)         |
| `title`         | Короткий заголовок                                | `string`                                      |
| `date`          | Дата події                                        | `YYYY-MM-DD` (ISO-8601)                       |
| `lang`          | Мова запису                                       | `ua` або `en`                                 |
| `source`        | Посилання на першоджерело                         | URL                                           |
| `summary`       | 200-300 слів                                      | `string`                                      |
| `mitre_attack`  | Список ID тактик/технік MITRE ATT&CK              | `array[string]`                               |
| `affected_sector` | Галузь, що постраждала                           | `enum`: `Energy`, `Agro`, `Transport`, `Government`, `Finance` |
| `cvss`          | Базова оцінка CVSS v3.1                           | `float` (0.0 – 10.0)                          |
| `tags`          | Додаткові ключові слова                           | `array[string]`                               |

> **Методологія:** анотацію виконано згідно з [MITRE ATT&CK](https://attack.mitre.org/) та [CVSS v3.1](https://www.first.org/cvss/).  
> Дані зібрані з публічних звітів CERT-UA, CISA, ENISA та провайдерів OT-безпеки.
