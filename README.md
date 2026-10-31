# Security Playbook — учебный набор по реагированию на инциденты

Личный учебный проект: план реагирования на инциденты (IR-план) и плейбуки для вымышленной компании «Альфа-Трейд» (интернет-магазин, ~300 сотрудников; NGFW, WAF, антивирус, EDR, SIEM, облачная почта).

> Учебный материал. Сроки уведомления регуляторов (152-ФЗ, 187-ФЗ) и другие нормативные детали нужно сверять с актуальными текстами законов.

## Структура

| Путь | Что внутри |
|---|---|
| [plan/ir-plan.md](plan/ir-plan.md) | IR-план: роли, уровни критичности, жизненный цикл инцидента, коммуникации |
| [playbooks/PB-00-template.md](playbooks/PB-00-template.md) | Шаблон плейбука |
| `playbooks/PB-01 … PB-10` | Топ-10 сценариев |
| `playbooks/PB-S1 … PB-S4` | Реагирование на сработки СЗИ: WAF, NGFW, антивирус, EDR |
| `reviews/` | Рецензии SOC-аналитика и инженера ИБ на каждый плейбук |

## Плейбуки

| Код | Сценарий |
|---|---|
| [PB-01](playbooks/PB-01-phishing.md) | Фишинговое письмо |
| [PB-02](playbooks/PB-02-ransomware.md) | Шифровальщик |
| [PB-03](playbooks/PB-03-account-compromise.md) | Компрометация учётной записи |
| [PB-04](playbooks/PB-04-malware-workstation.md) | Вредонос на рабочей станции |
| [PB-05](playbooks/PB-05-data-leak.md) | Утечка данных |
| [PB-06](playbooks/PB-06-ddos.md) | DDoS-атака |
| [PB-07](playbooks/PB-07-insider.md) | Инсайдер |
| [PB-08](playbooks/PB-08-web-app-breach.md) | Взлом веб-приложения |
| [PB-09](playbooks/PB-09-lost-device.md) | Потеря или кража устройства |
| [PB-10](playbooks/PB-10-cloud-account-compromise.md) | Компрометация облачного аккаунта |
| [PB-S1](playbooks/PB-S1-waf-alert.md) | Сработка WAF |
| [PB-S2](playbooks/PB-S2-ngfw-alert.md) | Сработка NGFW |
| [PB-S3](playbooks/PB-S3-antivirus-alert.md) | Сработка антивируса |
| [PB-S4](playbooks/PB-S4-edr-alert.md) | Сработка EDR |

## Основа

NIST SP 800-61, SANS PICERL, MITRE ATT&CK.
