## 🛒 **Ecommerce Retention Agent**

AI-powered customer retention workflow built with Lyzr

Identify → Decide → Personalize

## 💡 The Idea

Ecommerce teams don't need to message every customer.

This workflow identifies who needs attention, decides what action to take, and generates what to say.

⚙️ How It Works

Customer Data → Classify → Strategize → Personalize

📊 Agent 1 — Customer Classifier
Identifies customer risk using purchase behavior, spend and inactivity.

🎯 Agent 2 — Retention Strategist
Determines the appropriate action, channel and urgency.

✉️ Agent 3 — Message Generator
Creates personalized re-engagement messaging based on the strategy.

Architecture

 ![Ecommerce Retention Agent Workflow](assets/Flow.png)

🧪 Example

Aman — C035
48 days inactive · ₹45,000 spend · Luxury Watches

↓

High-Value At-Risk

↓

High-Value Retention · Email · Critical

↓

Personalized re-engagement message

🛠️ Tech Stack

Lyzr · LLMs · Prompt Engineering · Multi-Agent Workflows · Structured JSON

📊 Evaluation

Tested with 50 synthetic customer profiles, including:

Normal customer behavior
30/60-day boundary cases
High-value customers
Low-frequency / high-spend customers
Inconsistent data

Validated classification, strategy selection, structured outputs and message personalization.

## 🧠 Key Learnings

- Learned how to design and connect multi-agent workflows using Lyzr.
- Understood how to pass structured outputs between agents.
- Improved prompt design using clear rules, constraints, and edge-case handling.
- Learned the importance of defining strict output schemas for reliable agent responses.
- Explored how customer behavior can be translated into actionable retention strategie

## 🧪 Prompt Evaluation

Prompts were iteratively tested using normal and edge-case customer profiles.

Evaluation focused on:

- Classification consistency
- Correct handling of 30/60-day boundaries
- Retention strategy accuracy
- Channel and urgency consistency
- Customer-data preservation
- Message personalization
- Preventing unsupported discounts/offers

The prompts were refined based on observed failures before connecting the agents into the final workflow.

## 🚧 Challenges

1. Agent-to-agent context passing
Ensuring each agent receives the relevant output from the previous agent.

2. Schema mismatch
The initial generated schema used unrelated customer segments such as consumer and vip. This was corrected to match the business-specific retention segments.

3. Data preservation
Preventing agents from modifying customer IDs or reinterpreting classifications.

4. Edge cases
Handling customers exactly at inactivity boundaries and customers with unusual combinations of spend and purchase frequency.

5. Cost-efficient testing
Used targeted test cases during development and reserved broader testing for the final workflow to minimize LLM usage costs.

## 🚀 Future

Email automation → CRM integration → Campaign analytics
