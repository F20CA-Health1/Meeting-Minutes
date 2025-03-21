# Minutes

Note: Meeting online during several sudden problems

Present: Ka2023, rv2009, zj2009, lh2020

Minutes taken by: zj2009

## Agenda

- Discuss presentation feedback and changes that may need to be made regarding it
- Update project health of each sub-component and evaluate deadlines

# Topics

## Presentation Feedback

- Deeper safety analysis explanation
- Decision on local models needs to be made

## RAG Performance

- Maybe scale back RAG performance analysis to only look at one (or a few) models as performance may vary drastically between them.

## Evaluation

- Add evaluation for other components to plan.
  - Not a must, but good.

- For each component, draft short plan of how it would be evaluated.

### Heuristic Analysis

- User-friendliness benchmark (check interaction design for standard form name)

## Safety

- Testing more models, require GPU which zj2009 will provide this week.

## Local Model Choices:

- Llama3: 8b
  - Variants such as Llama3-Med
- Deepseek: 7b

### Finetuning models

- MED42-V2

## Cloud Model Choices

- Any cloud model (such as GPT-4) will need sufficient guard-rails support NOT included as it will prevent medical advice etc.

## Progress Report

### RAG

### Safety

Safety and performance reconfirmation done.

Needs to be turned into module that queries whether agent response is safe etc.

Pre/Post finetuning safety analysis should be carried out aswell.

### TTS

Local Package / Function

Provide comparison two different models/services.

### Safety Agent

Nearly finished. This runs during the conversation unlike prior which is finished performance evaluation over conversation.

More tuned towards safe conversation than conversation model.

## Integration

Skeleton out modules, feeding input from one into the other.

# Questions for Meeting

- Cloud models with safety features that wont interact with task
- What kind of demo video?
- Conference paper writing:
  - Sections
  - Which parts need focus
  - How many reference
  - How long



