# Полезные репозитории: готовые плейбуки и инструменты

Подборка открытых проектов на GitHub для изучения реагирования на инциденты. Ссылки проверены 31.10.2026. Это внешние проекты, перед запуском любого инструмента читайте его документацию и лицензию и пробуйте сначала в лабораторном стенде.

## 1. Готовые плейбуки и методологии

| Репозиторий | Что внутри | Чем полезен для учёбы |
|---|---|---|
| [certsocietegenerale/IRM](https://github.com/certsocietegenerale/IRM) | Incident Response Methodologies от CERT Société Générale: короткие карточки по 6 фазам (подготовка, обнаружение, сдерживание, устранение, восстановление, уроки) | Классика жанра. Хорошо сравнивать со своими PB-01…PB-10: фишинг, шифровальщик, DDoS, утечка, вредонос на Windows/Linux и т.д. |
| [austinsonger/Incident-Playbook](https://github.com/austinsonger/Incident-Playbook) | Плейбуки, привязанные к техникам MITRE ATT&CK (T1486 Ransomware, T1133 VPN, T1055 Process Injection…) плюс battle cards | Показывает, как строить плейбук от техники атакующего, а не от типа инцидента |
| [guardsight/gsvsoc_cirt-playbook-battle-cards](https://github.com/guardsight/gsvsoc_cirt-playbook-battle-cards) | Одностраничные PDF-карточки по техникам ATT&CK (Pass the Hash, VSS deletion, persistence…) | Формат «шпаргалки на одну страницу» для L1/L2 |
| [counteractive/incident-response-plan-template](https://github.com/counteractive/incident-response-plan-template) | Шаблон IR-плана и набор плейбуков в Markdown | Удобно сравнить со своим `plan/ir-plan.md`: структура ролей, фаз, коммуникаций |
| [LetsDefend/incident-response-playbooks](https://github.com/LetsDefend/incident-response-playbooks) | Плейбуки от учебной SOC-платформы LetsDefend | Ориентированы на начинающих аналитиков, стыкуются с их учебными алертами |
| [luduslibrum/awesome-playbooks](https://github.com/luduslibrum/awesome-playbooks) | Каталог ссылок на плейбуки разных организаций | Точка входа: найти плейбуки от CISA, Microsoft, AWS и др. |
| [msraju/Incident-Response-Playbooks](https://github.com/msraju/Incident-Response-Playbooks) | Сборник плейбуков по типовым сценариям | Ещё один взгляд на те же сценарии |
| [jacobtaylorsec/soc-runbook](https://github.com/jacobtaylorsec/soc-runbook) | SOC-ранбуки с запросами Splunk (SSH brute force, фишинг, вредонос, облако) | Пример плейбуков с конкретными SIEM-запросами |

## 2. Плейбуки автоматизации (SOAR)

| Репозиторий | Что внутри |
|---|---|
| [correlatedsecurity/Awesome-SOAR](https://github.com/correlatedsecurity/Awesome-SOAR) | Каталог SOAR-платформ, плейбуков и интеграций |
| [Azure/Azure-Sentinel](https://github.com/Azure/Azure-Sentinel) | Официальный репозиторий Microsoft Sentinel: правила, запросы KQL, плейбуки на Logic Apps (папки `Playbooks` и `Solutions/*/Playbooks`) |
| [Bert-JanP/Sentinel-Automation](https://github.com/Bert-JanP/Sentinel-Automation) | Плейбуки Sentinel для обогащения и анализа инцидентов |

## 3. Инструменты: сбор артефактов и триаж

| Репозиторий | Для чего |
|---|---|
| [Velocidex/velociraptor](https://github.com/Velocidex/velociraptor) | Сбор артефактов и охота за угрозами на тысячах хостов. Бесплатная альтернатива части функций EDR |
| [Digital-Defense-Institute/triage.zip](https://github.com/Digital-Defense-Institute/triage.zip) | Готовый настроенный коллектор Velociraptor для быстрого триажа |
| [tclahr/uac](https://github.com/tclahr/uac) | Сбор артефактов с Linux, macOS, ESXi, BSD и др. (Unix-like Artifacts Collector) |
| [ANSSI-FR/DFIR-ORC](https://github.com/ANSSI-FR/DFIR-ORC) | Сборщик артефактов Windows от французского ANSSI |
| [EricZimmerman/KapeFiles](https://github.com/EricZimmerman/KapeFiles) | Цели и модули для KAPE (сам KAPE скачивается с сайта Kroll) |

## 4. Инструменты: анализ логов, памяти и таймлайнов

| Репозиторий | Для чего |
|---|---|
| [Yamato-Security/hayabusa](https://github.com/Yamato-Security/hayabusa) | Быстрый анализ журналов Windows (EVTX) по Sigma-правилам и построение таймлайна |
| [WithSecureLabs/chainsaw](https://github.com/WithSecureLabs/chainsaw) | Быстрый поиск и охота по EVTX и другим артефактам Windows |
| [SigmaHQ/sigma](https://github.com/SigmaHQ/sigma) | Открытый формат и тысячи правил детектирования, конвертируются под любой SIEM |
| [volatilityfoundation/volatility3](https://github.com/volatilityfoundation/volatility3) | Анализ дампов оперативной памяти |
| [log2timeline/plaso](https://github.com/log2timeline/plaso) | Супер-таймлайн из множества артефактов |
| [EricZimmerman](https://github.com/EricZimmerman) | Набор утилит Эрика Циммермана для разбора артефактов Windows (реестр, prefetch, MFT, jump lists) |
| [Neo23x0/Loki](https://github.com/Neo23x0/Loki) | Простой сканер IOC и YARA-правил |
| [VirusTotal/yara](https://github.com/VirusTotal/yara) | YARA: описание и поиск вредоносных файлов по шаблонам |

## 5. Платформы ведения инцидентов и TI

| Репозиторий | Для чего |
|---|---|
| [dfir-iris/iris-web](https://github.com/dfir-iris/iris-web) | Совместная работа над инцидентом: кейсы, таймлайн, IOC, задачи |
| [TheHive-Project](https://github.com/TheHive-Project) | TheHive и Cortex: кейс-менеджмент и обогащение. Новые версии развивает [StrangeBee](https://github.com/StrangeBeeCorp), лицензия изменилась, проверяйте условия |
| [MISP/MISP](https://github.com/MISP/MISP) | Платформа обмена индикаторами компрометации |
| [Shuffle/Shuffle](https://github.com/Shuffle/Shuffle) | Открытый SOAR для автоматизации плейбуков |
| [wazuh/wazuh](https://github.com/wazuh/wazuh) | Открытый SIEM/XDR, удобен для домашней лаборатории |

## 6. Тренировка и проверка детектов

| Репозиторий | Для чего |
|---|---|
| [redcanaryco/atomic-red-team](https://github.com/redcanaryco/atomic-red-team) | Маленькие тесты техник ATT&CK: запустили в лабе, проверили, сработал ли алерт и плейбук |
| [mitre-attack/attack-navigator](https://github.com/mitre-attack/attack-navigator) | Карта покрытия техник ATT&CK вашими детектами и плейбуками |

## 7. Большие каталоги (awesome-списки)

- [meirwah/awesome-incident-response](https://github.com/meirwah/awesome-incident-response): главный список инструментов IR
- [cugu/awesome-forensics](https://github.com/cugu/awesome-forensics): инструменты цифровой криминалистики
- [forensicfellowship/Open_Source_DFIR_Tools](https://github.com/forensicfellowship/Open_Source_DFIR_Tools): открытые DFIR-инструменты
- Темы GitHub: [incident-response-playbook](https://github.com/topics/incident-response-playbook), [incident-response-plan](https://github.com/topics/incident-response-plan)

## Как этим пользоваться при учёбе

1. Возьмите свой плейбук, например `PB-02-ransomware.md`, и откройте аналог в IRM и в Incident-Playbook (T1486). Выпишите, чего у вас нет.
2. Поднимите лабу: Wazuh или Velociraptor на 1–2 виртуалках, Atomic Red Team для имитации атаки.
3. Прогоните плейбук по шагам: найдите алерт, соберите артефакты Velociraptor/UAC, разберите журналы Hayabusa/Chainsaw.
4. Добавьте найденные пробелы в свой плейбук.

## Не на GitHub, но обязательно к прочтению

- NIST SP 800-61 Rev. 3 (Incident Response Recommendations) — csrc.nist.gov
- CISA Federal Government Cybersecurity Incident & Vulnerability Response Playbooks — cisa.gov
- Microsoft Incident Response playbooks (фишинг, password spray, app consent grant) — learn.microsoft.com
