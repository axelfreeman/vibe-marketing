# What are tokens in a neural network простыми словами

> **TL;DR:** A token is a unit of exchange of letters for computation. You submit a question of 40 characters — the neural network spends tokens to "read" it. Then it generates a response of 2000 characters — spending more tokens. Total: ~2040 tokens per request. Free models provide a daily token limit, paid ones — unlimited.

Что такое токены в нейросети

Короткий ответ:
A token is a unit of exchange of letters for computation. You submit a question of 40 characters — the neural network spends tokens to "read" it. Then it generates a response of 2000 characters — spending more tokens. Total: ~2040 tokens per request. Free models provide a daily token limit, paid ones — unlimited.

Tokens are the currency of neural networks.

Every time you write something in ChatGPT or DeepSeek, you spend tokens. It’s like gasoline for a car. A query is spent tokens. A response is also spent tokens. The entire conversation in a session is the sum of tokens.

Free models (DeepSeek Chat, ChatGPT Free) have a daily limit — typically 50-100 requests. Paid models (ChatGPT Plus, Claude Pro) are unlimited within reasonable bounds. API access (for business) charges per token, from $0.0001 to $0.015 per 1000 tokens.

One token ≠ one word

Example of tokenization:

Привет, как дела?

→ [При][вет][,][ как][ дел][а][?] = 
7 токенов

Hello, how are you?

→ [Hello][,][ how][ are][ you][?] = 
6 токенов

In Russian, one word is approximately 2–3 tokens. In English, it’s ~1.3 tokens. Therefore, communicating in English is slightly cheaper. Long compound words like “достопримечательность” can take 5–6 tokens.

Context window: why it matters

Each model has a limit on how many tokens it can "see" at once. This is called the context window.

Модель

Контекст

Примерно страниц

Цена

DeepSeek Chat

128K

~300

Free

ChatGPT 4o

128K

~300

$20/мес

Claude 3.5

200K

~500

$20/мес

Gemini 2.5

1M

~2500

$20/мес

Всё что не влезло в контекстное окно — «забывается». Именно поэтому в длинных диалогах нейросеть может потерять нить разговора — ранние сообщения выпали из окна.

Как экономить токены

Write короче.
 Убирайте «не мог бы ты пожалуйста» — нейросети не нужна вежливость, ей нужна чёткость

Не просите повторять вопрос в ответе.
 Это тратит токены на дублирование

Используйте модели с большим контекстом.
 DeepSeek даёт 128K бесплатно — хватит для большинства задач

Начинайте новый чат для новой темы.
 Не копите историю — модель будет тратить токены на её обработку

I'll set up API-доступ к 60+ моделям с оптимальным расходом токенов под ваш бюджет. От 500€.

Discuss →