# RESOLVA Assist – AI Claims Copilot

Transforming 23 years of frontline claims expertise into AI guidance for the next generation of insurance professionals.

## Overview

RESOLVA Assist is an AI-powered decision support system designed to support junior automobile insurance claims handlers.

It helps users identify missing information, organize the next step, and make more consistent decisions during complex claims handling situations.

Rather than replacing human judgment, RESOLVA Assist provides structured guidance so that claims professionals can make better-informed decisions while retaining responsibility for the final outcome.

## The Problem

Claims handling requires more than following a manual.

Junior professionals must interpret incomplete information, separate facts from customer expectations, identify what still needs to be confirmed, and decide what action should come next.

Much of this judgment is developed through years of frontline experience and is often difficult to transfer through manuals or classroom training alone.

At the same time, experienced supervisors spend a significant amount of time reviewing claim histories, checking for missing information, correcting mistakes, and explaining the next step.

RESOLVA Assist was created to make this practical judgment more accessible and repeatable.

## What It Does

RESOLVA Assist analyzes a claims-handling situation and provides concise operational guidance.

It can help users:

- Identify missing or unclear information
- Organize the facts of the case
- Separate customer requests from verified facts
- Determine the next information to confirm
- Suggest the next practical action
- Avoid unsupported assumptions
- Provide short and consistent explanation examples
- Support junior staff learning through real-world scenarios

The current prototype focuses on complex automobile insurance scenarios, including replacement vehicle situations and no-fault claim discussions.

## Who It Helps

RESOLVA Assist is primarily designed for:

- Junior claims handlers
- Training managers
- Supervisors
- Experienced claims professionals
- Insurance agents supporting customers

The greatest organizational value may be for education managers and supervisors, who need to maintain consistent claims-handling quality while supporting less experienced staff.

## How It Works

Users enter the details of a claims-handling situation.

The system classifies the issue, checks which information is known or missing, and routes the case through structured decision logic.

It then returns concise guidance focused on:

1. What has been confirmed
2. What still needs to be checked
3. What action should come next
4. What explanation can be given to the customer
5. What expressions or assumptions should be avoided

The system is designed to support decision-making without inventing facts that were not included in the original input.

## Example Use Case

A junior claims handler receives a call from a customer who may need a replacement vehicle, but the liability position, repair status, vehicle usability, and current rental status are not yet fully confirmed.

Instead of giving a premature answer, RESOLVA Assist helps the handler identify the missing information, organize the case, and determine the appropriate next step.

This reduces inconsistent explanations and helps prevent avoidable mistakes.

## Why I Built It

I spent 23 years working in automobile insurance claims, including frontline claims handling, negotiation, management, recruitment, and junior employee training.

Over time, I saw how much valuable professional judgment remained inside individual employees and how difficult it was to transfer that knowledge consistently.

I also saw many young employees leave the industry before they had enough time to develop confidence and practical judgment.

I built RESOLVA Assist because valuable frontline experience should not disappear when experienced professionals leave an organization or change careers.

AI makes it possible to transform tacit professional knowledge into structured guidance that can support the next generation.

## Development Approach

RESOLVA Assist was built through a combination of:

- Dify workflow development
- Structured decision logic
- AI-assisted coding
- Repeated scenario testing
- Manual review based on frontline claims experience

The main technical challenge was not writing code.

The most difficult part was reproducing professional judgment: determining which facts matter, which questions should come next, what should not be assumed, and how to guide a junior employee without removing human responsibility.

## Current Status

The current prototype includes structured decision support for automobile insurance claims scenarios.

Development has included:

- Scenario classification
- Branching decision logic
- Input normalization
- Missing-information detection
- Pushback and follow-up handling
- Automated test cases
- Manual scenario validation

The system is still under active development and is being expanded through additional scenarios and testing.

## Built With

- Dify
- AI-assisted development
- JavaScript-based classification logic
- Structured workflow design
- Scenario-based testing

## What I Learned

This project showed me that domain expertise can become a software asset.

A non-engineer can build a meaningful AI system when practical experience is carefully structured into:

- Decision rules
- Classification criteria
- Exception handling
- Escalation logic
- Consistent response patterns

The value does not come from AI alone.

It comes from combining AI with deep frontline context.

## What’s Next

The next stage of RESOLVA Assist is a real-time AI copilot for claims professionals.

The long-term vision is a system that can understand the claim history before a call, listen to the conversation in real time, and suggest the next best action while the claims handler remains in control.

Future development will focus on:

- Expanding supported claims scenarios
- Improving real-time decision support
- Integrating claim history and conversation context
- Testing with actual claims professionals
- Building a production-ready interface
- Adapting the framework to other operational decision-support fields

## Human Responsibility

RESOLVA Assist is designed to support professional judgment, not replace it.

AI should perform as much analysis and support work as possible, while the final decision and responsibility remain with the human professional.

## Project Vision

Preserve valuable frontline expertise.

Make professional judgment easier to transfer.

Help the next generation make better decisions.
## Quick Start

### Live Demo

No installation is required.

Open the Live Demo:
(URL)

Copy one of the sample inputs.

Submit.

Compare the output with the expected behavior.

### Local Development

1. Clone this repository.
2. Import the Dify workflow.
3. Configure your LLM API key.
4. Publish the workflow.
5. Run the included test scenarios.
   
## Sample Inputs

Scenario 1

My car cannot be driven after the accident.
Liability has not been determined.
Can I get a rental car?

Expected behavior

• Detect replacement vehicle inquiry
• Detect unknown liability
• Avoid guaranteeing payment
• Explain next step

## How GPT-5.6 and Codex Were Used

GPT-5.6 served as a design and reasoning partner throughout the project.

It was used to:

• Convert practical insurance knowledge into structured decision rules
• Design response principles
• Review difficult edge cases
• Improve English documentation

Codex accelerated implementation by:

• Writing and revising JavaScript classifier logic
• Expanding keyword coverage
• Generating automated test cases
• Detecting routing regressions
• Speeding up iterative development

Final business decisions remained under human control and were based on 23 years of automobile claims experience.

## Key Design Decisions

Several important decisions were intentionally implemented.

Examples include:

• Never assume facts that are not explicitly stated.
• Never guarantee rental reimbursement while liability remains unresolved.
• Separate customer statements from verified facts.
• Prioritize operational guidance over lengthy legal explanations.
• Keep humans responsible for final decisions.

These principles were derived from practical claims-handling experience rather than generic chatbot behavior.

## Live Demo

Try the live demo here:

https://udify.app/chat/27pWfgsdddFyqwYy

The current prototype accepts Japanese input.

You can copy and paste one of the following examples.

Example 1

車が動かないです。
過失割合はまだ決まっていません。
代車は借りられますか？

Expected behavior

- Detects a replacement vehicle inquiry
- Detects that the vehicle is not drivable
- Detects that liability is still undetermined
- Provides practical next-step guidance

Example 2

私は悪くありません。
相手が全部悪いです。

Expected behavior

- Detects a policyholder zero-liability claim
- Explains the next procedural step
- Avoids making a final liability determination
