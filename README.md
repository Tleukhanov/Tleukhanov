<div align="center">

<a href="https://github.com/Tleukhanov">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=30&duration=3000&pause=1000&color=2ECC71&center=true&vCenter=true&multiline=true&repeat=true&width=700&height=120&lines=%F0%9F%96%A5%EF%B8%8F+Yeraly+Tleukhanov%3B+AI+Engineer+%28Python%29%3B+LLM+%C2%B7+RAG+%C2%B7+FastAPI+%C2%B7+PostgreSQL" alt="Typing SVG" />
</a>

<br/>

<a href="https://github.com/Tleukhanov">
  <img src="https://komarev.com/ghpvc/?username=Tleukhanov&label=Profile%20Views&color=0e75b6&style=flat" alt="Profile Views" />
</a>

</div>

---

## About Me

```python
class Developer:
    def __init__(self):
        self.name     = "Yeraly Tleukhanov"
        self.role     = "AI Engineer (Python)"
        self.location = "Astana, Kazakhstan"
        self.focus    = ["LLM Integration", "RAG", "Conversational AI", "Applied ML"]
        self.stack    = ["Python", "FastAPI", "PostgreSQL", "OpenRouter"]
```

---

## Commercial Experience

**TeenFreelance (startup)** — Backend + ML Engineer, 2026
- Backend фриланс-платформы: Python, FastAPI, PostgreSQL, SQLAlchemy, Alembic, pytest (65 тестов), CI
- Рекомендательный движок подбора исполнителей (backend-фича): топ-N кандидатов по проценту совпадения
- Классификатор модерации описаний заказов (TF-IDF + Logistic Regression): отсеивает ТЗ с попыткой увода
  с платформы и невнятные ТЗ → модератору либо AI-улучшение
- Реальных данных не существовало → синтетический датасет. Провёл бенчмарк генераторов (Kimi vs DeepSeek),
  обнаружил **mode collapse** у Kimi → переобучение; добавил разнообразие против shortcut learning
- Тест-сет: часть примеров написал вручную, включая попытки обхода (`tg`, `whatsapp`) — детектор их ловил
- ROC-AUC **0.90 на валидации / 0.80 на тесте**. **В прод осознанно не внедрил** — жду реальные данные,
  потому что метрика на синтетике ≠ работа на живых людях
- LLM-фича «улучшить ТЗ» (OpenAI-совместимый API, предложение без записи в БД)
- Закрыл 3 IDOR-уязвимости, написал документацию API для фронта
- Git-флоу: feature-ветки, code review, Pull Requests

---

## Tech Stack

<div align="center">

#### Languages
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

#### Backend & Frameworks
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![aiogram](https://img.shields.io/badge/aiogram_3.x-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)

#### AI & LLM
![OpenRouter](https://img.shields.io/badge/OpenRouter-6467F2?style=for-the-badge&logo=openai&logoColor=white)
![RAG](https://img.shields.io/badge/RAG-7C3AED?style=for-the-badge)
![Prompt Engineering](https://img.shields.io/badge/Prompt_Engineering-0E7C3E?style=for-the-badge)
![Embeddings](https://img.shields.io/badge/Embeddings-9333EA?style=for-the-badge)
![ONNX Runtime](https://img.shields.io/badge/ONNX_Runtime-005CED?style=for-the-badge&logo=onnx&logoColor=white)

#### ML & Data Science
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![CatBoost](https://img.shields.io/badge/CatBoost-F6C915?style=for-the-badge&logoColor=black)
![XGBoost](https://img.shields.io/badge/XGBoost-EC6C00?style=for-the-badge&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

#### Databases & DevOps
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)

</div>

---

## Featured Projects

<table>
<tr>
<td width="50%">

### AdaptENG
Персональный AI-репетитор английского: адаптивные уроки, диагностика уровня A1–C1, голосовой контур (STT/TTS), достижения. Мульти-провайдерная LLM-фабрика (OpenAI, Gemini, Anthropic, Ollama), RAG по грамматике (54 правила) с цитатами и честными отказами, SRS по SM-2, **489 тестов**, CI с Postgres. Есть web-версия: FastAPI + Next.js.

**Stack:** Python, FastAPI, aiogram 3.x, Next.js, PostgreSQL, faster-whisper, edge-tts, pytest

[![Readme](https://img.shields.io/badge/README-blue?style=for-the-badge)](https://github.com/Tleukhanov/AdaptENG)

</td>
<td width="50%">

### chess_trainig_app
Персональный шахматный тренер: партии с Lichess → анализ Stockfish → объяснение ошибок через LLM → дебютный репертуар → дрели из собственных зевков. **Инференс нейросети Maia-2 через ONNX** с ручным энкодером доски (18 плоскостей), зеркалированием при ходе чёрных, маскированием легальных ходов и ленивой выгрузкой модели под лимит 512 МБ. **741 тест.**

**Stack:** Python, FastAPI, python-chess, Stockfish, ONNX Runtime, LLM, PostgreSQL

[![Readme](https://img.shields.io/badge/README-blue?style=for-the-badge)](https://github.com/Tleukhanov/chess_trainig_app)

</td>
</tr>
<tr>
<td width="50%">

### shorts-factory
Фабрика коротких видео поверх открытого пайплайна `random-or/shorts-clipper` (MIT). Моя часть — **159 файлов / ~39 400 строк, из них 75 файлов тестов**: шахматный модуль (PGN → решающий ход → отрисовка доски, Stockfish с честным фолбэком), stock-режим (оригинальные шорты без чужого видео), локальный Piper TTS, compliance gate, metrics store, отчёт по удержанию с грейдами A/B/C/D, TikTok-публикация, systemd-деплой.

**Stack:** Python, FFmpeg, faster-whisper, Stockfish, Piper TTS, systemd, GitHub Actions

[![Readme](https://img.shields.io/badge/README-blue?style=for-the-badge)](https://github.com/Tleukhanov/shorts-factory)

</td>
<td width="50%">

### Fair_Play_Detector
Сервис вероятностного анализа партий Lichess на признаки машиноподобной игры. Group-aware сплиты (по игроку, без пересечения групп), калибровка вероятностей, метрики: ROC-AUC, PR-AUC, recall@1%FPR, Brier, calibration curve. Пороги подбираются на валидации по max(precision×recall). Fail-closed гейт качества данных и sha256-хэш датасета. В README — честный разбор собственной утечки.

**Stack:** Python, FastAPI, SQLAlchemy, Alembic, scikit-learn, XGBoost, ONNX Runtime

[![Readme](https://img.shields.io/badge/README-blue?style=for-the-badge)](https://github.com/Tleukhanov/Fair_Play_Detector)

</td>
</tr>
<tr>
<td colspan="2">

### TeenFreelance 🔒
Бэкенд и ML для стартапа фриланс-платформы: рекомендательный движок (backend), классификатор модерации ТЗ (TF-IDF + LogReg, ROC-AUC 0.90/0.80), синтетический датасет с бенчмарком генераторов, LLM-улучшение текстов, 65 pytest-тестов и CI. Репозиторий приватный — доступ по запросу.

**Stack:** Python, FastAPI, PostgreSQL, SQLAlchemy, scikit-learn, pytest

[![GitHub](https://img.shields.io/badge/Access_on_request-grey?style=for-the-badge)](https://github.com/Tleukhanov)

</td>
</tr>
</table>

---

## GitHub Stats

<div align="center">

<a href="https://github.com/Tleukhanov">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=Tleukhanov&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" />
</a>
<a href="https://github.com/Tleukhanov">
  <img height="180em" src="https://github-readme-streak-stats.herokuapp.com/?user=Tleukhanov&theme=tokyonight&hide_border=true" />
</a>

</div>

<div align="center">

<a href="https://github.com/Tleukhanov">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Tleukhanov&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" />
</a>

</div>

<div align="center">

<a href="https://github.com/Tleukhanov">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Tleukhanov&theme=tokyonight&hide_border=true&area=true" alt="Activity Graph" />
</a>

</div>

---

## Contribution Snake

<div align="center">

![Snake animation](https://raw.githubusercontent.com/Tleukhanov/Tleukhanov/output/github-contribution-grid-snake-dark.svg)

</div>

---

## Contact

<div align="center">

Astana, Kazakhstan · tleukhanov0409@mail.ru

[![Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/Napaleonwww)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Tleukhanov)

</div>
