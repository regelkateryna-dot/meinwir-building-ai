# MeinWir — Family, Everyday Support, and Understanding the Person

*Building AI course project*

## Summary

MeinWir is a family app centred on an older person’s personal profile. It turns voice messages into confirmed requests, tasks, and reminders, helps overcome language barriers, and coordinates everyday support. A separate use case supports documentation in care facilities.

## Background

Everyday support involves many small tasks: buying household supplies, ordering personal hygiene products, checking bills, and arranging the delivery or return of mobility aids. When these responsibilities are scattered across conversations, messages, and separate calendars, information can get lost. Family members must repeatedly clarify who is responsible and whether a request has been fulfilled.

Older people may also find conventional smartphone interfaces difficult to use. Limited hand and finger mobility, pain, or tremors can make typing and tapping small buttons challenging. Voice interaction is therefore central to the MeinWir concept.

Care facilities face an additional challenge: staff must document their observations accurately. For employees whose first language differs from the language used for documentation, preparing written reports can require additional effort.

My motivation is to create an app that helps families understand one another, share responsibilities, and preserve the older person’s independence. The project centres on the individual’s wishes, habits, daily routines, and personal boundaries.

## How is it used?

### Family use case

An older person expresses a need by voice or text. For example:

> “The laundry detergent is almost finished. Please ask my daughter to buy some on Friday.”

AI prepares a clear task, identifying the request, intended recipient, and deadline. The user reviews the result and confirms that it should be shared. If the recipient or date is unclear, the app asks a follow-up question.

Once confirmed, the task appears for the selected family member, and its deadline is added to the calendar or reminders within MeinWir. The recipient can accept the task and mark it as completed. There is no need to enter the same information again in a separate calendar.

Other examples include:

- Reminders to buy groceries, household supplies, or personal hygiene products.
- Scheduling repeat orders for care supplies covered by insurance, where eligibility has been confirmed.
- Arranging the delivery, maintenance, or return of a rollator or wheelchair.
- Reminders about bills and payment deadlines, while leaving verification of payment details and payment itself to a person.
- Sharing everyday responsibilities among family members.

MeinWir is intended as a shared family space that connects communication with responsibility, deadlines, and outcomes. Its value lies in reducing the effort of organising support and helping maintain relationships between family members.

### Personal profile

The personal profile would contain preferences, habits, daily routines, and boundaries. For example:

> “Please knock before entering and wait for my reply.”

The user should control which information is visible to family members, a trusted person, or assigned care staff. Relatives should also be able to choose whether to receive tasks and reminders.

### Care facility use case

A staff member dictates observations in a language they are comfortable using. The system transcribes the speech and prepares a structured draft report in German.

Before saving it, the staff member checks the source content, translation, names, times, and other essential details. The system should flag unclear or missing information and request clarification rather than invent facts.

The aim is to make documentation easier and reduce duplicate data entry. Actual time savings and documentation quality would need to be evaluated separately.

## Data sources and AI methods

The educational prototype will use **fictional profiles, messages, bills, and sample reports**. Real personal information about older people or care staff is not needed for the initial evaluation.

Planned AI methods include:

- **Speech recognition:** converting voice messages into text.
- **Natural language processing:** identifying requests, items, dates, and explicitly named recipients.
- **Machine translation:** supporting communication across languages and preparing German documentation drafts.
- **Language models:** producing clear task descriptions or report drafts while preserving the original meaning.

After confirmation, conventional application logic would create tasks and calendar reminders. Recurring deadlines could follow user-defined rules without requiring AI for every occurrence.

Potential data sources include user messages, selected profile information, and dates entered by the user. Documents or bills would only be processed with specific permission, and extracted information would require review.

## Challenges

Speech recognition and translation errors can change the meaning of a message, particularly negations, dates, and personal wishes. Important actions therefore require clear confirmation. Users must be able to correct or cancel a task.

Voice interaction will not suit everyone. Speech and hearing impairments, different accents, and background noise must be considered. Text input, large controls, and accessible ways to review results should remain available.

MeinWir is not intended for emergency response, diagnosis, treatment recommendations, or autonomous care decisions. It does not determine insurance eligibility, pay bills automatically, or guarantee that a task will be completed.

Personal profiles and care reports may contain sensitive information. Before real-world use, the project must establish appropriate grounds for processing, minimise collected data, assess AI service providers, and implement access controls, secure storage, and deletion procedures. Family and professional care settings require separate access arrangements.

For care documentation, staff must retain responsibility for the final report. It should also be possible to trace changes made after dictation.

## What next?

The first step is to evaluate one complete family workflow:

**Voice request → clear draft → user confirmation → task and reminder → completion response.**

Evaluation will begin with fictional data. It will examine whether meaning is preserved, dates and recipients are correct, how many corrections are needed, and whether the interface is usable for people with limited hand mobility.

A later stage could involve voluntary testing with older people and family members. The aim would be to learn whether MeinWir helps distribute responsibilities and reduces forgotten requests.

The care facility use case would be developed separately with care staff and relevant specialists. Evaluation would compare documentation time and meaning-related errors, alongside requirements for professional documentation and data protection.

**This description presents a concept and development plan. It does not imply that all described features have already been implemented or validated in real-world use.**

## Acknowledgments

MeinWir is an original project concept presented as a final project for the Building AI course by the University of Helsinki and MinnaLearn.

An AI assistant helped structure and edit this description. Any third-party code, models, images, or datasets used in the project will be credited, with their sources and licence terms identified.
