# Why neural networks lie and hallucinate

> **TL;DR:** Neural networks lie for three reasons: imperfect training data, limited context, and the absence of built-in fact-checking. They don’t verify truth—they predict text that sounds plausible.

Почему нейросети врут и галлюцинируют

Короткий ответ:
Neural networks lie for three reasons: imperfect training data, limited context, and the absence of built-in fact-checking. They don’t verify truth—they predict text that sounds plausible.

Reason #1: dirty data

The neural network learns from the internet. And the internet is full of errors, fakes, outdated information, and outright nonsense. When you ask "who invented the radio," the model may output Popov, Marconi, or Tesla — because all three versions were present in the training data. It doesn't know who is correct — it knows that people write about all three.

It’s like teaching a student from textbooks where half the facts are mixed up. The student will pass the exam, but half the answers will be wrong. It’s the same with neural networks.

Reason #2: limited context

Each neural network has a "context window"—the amount of text it can hold in memory at once. In 2024, this was 4–8K tokens (a couple of pages). By 2026, it will be 128–200K tokens (an entire book). But even 200K tokens is not infinite. If a conversation is long, the neural network "forgets" the beginning of the exchange and starts responding irrelevantly.

The context problem from six months ago is now being actively resolved. Gemini 2.5 handles 1M tokens — that's like "War and Peace" twice over. But fact-checking is still a weak point.

Reason #3: lack of fact-checking

A neural network does not search Google. It does not verify facts. It predicts the next word. When you ask, "How much is a ticket to Mars," it does not go to the SpaceX website—it "extrapolates" an answer based on what it has read on the internet. The result: a plausible but fictitious price.

Именно поэтому появились инструменты вроде Perplexity — они совмещают нейросеть с поиском. Модель сначала ищет источники, потом читает их, и только потом отвечает. Процент галлюцинаций падает в 3-5 раз.

Как с этим работать

Для фактов:
 используйте Perplexity или поисковые модели. Они показывают источники — можно проверить.

Для творчества:
 нейросети идеальны. Тексты, идеи, креативы — здесь галлюцинации это фича а не баг. Нейросеть «придумала» интересный заголовок? Отлично — это не ошибка, это креатив.

Для бизнеса:
 настройте RAG (Retrieval-Augmented Generation) — нейросеть будет искать ответы в вашей базе знаний а не «придумывать». Это снижает процент ошибок до 1-2%.

I'll set up RAG под ваш бизнес — нейросеть перестанет врать про ваши продукты. От 500€.

Discuss →